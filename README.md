# Instructions for developers

## Requisites

1. Install nodejs: [https://github.com/joyent/node/wiki/installing-node.js-via-package-manager]
2. Install npm: [https://www.npmjs.org/doc/README.html]
3. Install bower: `sudo npm install -g --save-dev bower`
4. Install gulp: `sudo npm install -g --save-dev gulp`
5. Install gulp bower for the plugin: Go to the plugin directory and execute: `sudo npm install --save-dev gulp-bower`

## Install the Mailchimp API for the first time

1. Open the console.
2. Go to the plugin directory
3. Execute `gulp install`

Mailchimp API Wrapper should have been installed in mailchimp-api folder

## Update Mailchimp API

Just run `gulp update`

## Notes

Try not to touch the Mailchimp classes, there's another class that makes all the work: mailchimp-api/mailchimp-api.php

This class extends from the main Mailchimp class and overrides several methods but uses WordPress functions instead.
