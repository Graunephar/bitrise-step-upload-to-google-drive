# Upload To Google Drive

Uploads selected files to a folder in Google Drive

# Inputs

## Service Account Credentials

You will need a Google Drive project for this step to work. The Google Drive project should have the Google Drive API enabled. Read how to do that [here](https://developers.google.com/drive/api/guides/enable-drive-api)

Also remember to share the folder you want to upload your files to with the service account. You can use the same sharing process as if you were sharing the files with a human user for this. Just share them with the email address of the service account.

* Create a new service account as described here. It does not need any roles or permissions
* Open the new service accounts, under the 'Keys' tap click 'Add Key'. Choose 'Create New Key'. And Choose key type 'JSON' in the popup. Save the json file somewhere on your computer




Read more about service accounts [here](https://developers.google.com/identity/protocols/oauth2/service-account)


## How to use this Step

Can be run directly with the [bitrise CLI](https://github.com/bitrise-io/bitrise),
just `git clone` this repository, `cd` into it's folder in your Terminal/Command Line
and call `bitrise run test`.

*Check the `bitrise.yml` file for required inputs which have to be
added to your `.bitrise.secrets.yml` file!*
