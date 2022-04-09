# Upload To Google Drive

Uploads selected files to a folder in Google Drive. Basically just a wrapper for [this](https://github.com/prasmussen/gdrive) really convenient Google Drive CLI client found

# Inputs

This is a detailed description of each input that the step needs. s

## Path to file(s) to upload

The relative path to one or more files that you want to upload. If multiple files seperatWe e each path by \n

## Folder ID
The folder id, is the ID of the folder you want to upload files to. The easiest way to find it is to inspect the folder in Google Drive in a browser. The ID is the last part of the url seen after the last `/`

## Service Account Credentials

You will need a Google Drive project for this step to work. The Google Drive project should have the Google Drive API enabled. Read how to do that [here](https://developers.google.com/drive/api/guides/enable-drive-api)

Also remember to share the folder you want to upload your files to with the service account. You can use the same sharing process as if you were sharing the files with a human user for this. Just share them with the email address of the service account.

* Create a new service account as described here. It does not need any roles or permissions
* Open the new service accounts, under the 'Keys' tap click 'Add Key'. Choose 'Create New Key'. And Choose key type 'JSON' in the popup. Save the json file somewhere on your computer
* In Bitrise under the 'Code Signing' tab upload the file and provide the name of the environment variable in the




Read more about service accounts [here](https://developers.google.com/identity/protocols/oauth2/service-account)


## How to use this Step

Can be run directly with the [bitrise CLI](https://github.com/bitrise-io/bitrise),
just `git clone` this repository, `cd` into it's folder in your Terminal/Command Line
and call `bitrise run test`.

*Check the `bitrise.yml` file for required inputs which have to be
added to your `.bitrise.secrets.yml` file!*
