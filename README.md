  

# Postman Test for Abstracta

This is a repository of export files for postman. this project have 2 files:

- abstracta.postman_collection.json
	- this file is the endpoints and test for each enpoint
- env.petStore.postman_environment.json
	- This file is the enviorment Variables

## Import in Postman
### Install postman: 
First of all, you will need install postman on your computer, to do this go to [postman website](https://www.postman.com/downloads/) and install.

### Import json files.
You have to import this 2 files to work propertly. 
To do this, open postman software and click on import button 

<img src="https://kibit.cl/fotos/SCR-20230723-nckp.png" />

Then will prompt you a pop up to upload the two files from this project. 

Once the files are loaded, this should appear confirming what is about to be imported. if all correct, press the orange button "import"
*The importat here is you can verify the file will import as collection and Enviroment, this will be detected automatically.*

<img src="https://kibit.cl/fotos/SCR-20230723-rmrs.png"/>

## Run Test with newman

You can run the test with [newman](https://www.npmjs.com/package/newman) package from NPM.
To do this you have to install this package on your local and run the test file with the enviroment

### install
To run Newman, ensure that you have Node.js >= v10.  [Install Node.js via package manager](https://nodejs.org/en/download/package-manager/).

### Installation

The easiest way to install Newman is using NPM. If you have Node.js installed, it is most likely that you have NPM installed as well.

    $ npm install -g newman

This installs Newman globally on your system allowing you to run it from anywhere. If you want to install it locally, Just remove the  `-g`  flag.

#### Using Homebrew

Install Newman globally on your system using Homebrew.

    $ brew install newman

## Usage

### Using Newman CLI

The  `newman run`  command allows you to specify a collection to be run. You can easily export your Postman Collection as a json file from the  [Postman App](https://www.postman.com/downloads/)  and run it using Newman.

    $ newman run abstracta.postman_collection.json -e env.petStore.postman_environment.json

For the complete list of options, refer the  [Command Line Options](https://www.npmjs.com/package/newman#command-line-options)  section below.

![terminal-demo](https://raw.githubusercontent.com/postmanlabs/postmanlabs.github.io/develop/global-artefacts/newman-terminal.gif)

