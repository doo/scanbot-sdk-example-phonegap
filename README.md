# Capture documents (OCR), barcodes, QR codes, MRZ and more.

## Scanbot SDK example app for PhoneGap

This example app demonstrates how to integrate the Scanbot SDK Cordova Plugin with PhoneGap.
The Scanbot SDK Cordova Plugin is available as [npm package](https://www.npmjs.com/package/cordova-plugin-scanbot-sdk).

The app demonstrates only a few features of the plugin. For more details please see this [documentation](https://scanbotsdk.github.io/documentation/cordova/).


## What is Scanbot SDK?
The Scanbot SDK brings scanning and document creation capabilities to your mobile apps.
It contains modules which are individually licensable as license packages.
For more details visit our website https://scanbot.io/sdk


## How to run this app

Install [PhoneGap](https://phonegap.com), fetch this repository and navigate to the project directory.

`cd scanbot-sdk-example-phonegap`

Install platforms and plugins (defined in the config.xml of this app):

`phonegap prepare`


Check installed platforms and plugins:

`phonegap platform ls`

`phonegap plugin ls`

You should see *android* and *ios* as installed platforms and *cordova-plugin-scanbot-sdk* as installed plugins.


Connect a device via USB and run the app.

Android:

`phonegap run android --device --verbose`

iOS:

To run this example app on an iOS device you have to adjust some settings in Xcode:
- *Provisioning* and *Code Signing* settings - see [Cordova docs](https://cordova.apache.org/docs/en/latest/guide/platforms/ios/index.html)
- Make sure *ScanbotSDK.framework* was added as Embedded Binary - see our [plugin docs](https://scanbotsdk.github.io/documentation/cordova/)

Then you can start the App in Xcode or via

`phonegap run ios --device --verbose`


## Please note

It is **not possible** to test or preview the features of the Scanbot SDK Cordova Plugin within the *PhoneGap Developer App*.

It is also **not possible** to test or preview the Scanbot SDK Cordova Plugin in a desktop browser.

Or in other words, the PhoneGap serve mode `phonegap serve` **will not work**! You have to build your app and deploy it on the target mobile device (`phonegap run android | ios`).


## Scanbot SDK trial mode

This example app does not contain a Scanbot SDK license key and runs in a **trial mode (trial period of 1 minute)**!  
After the trial period has expired the Scanbot SDK functions will stop working. 
The UI parts (like Camera UI) will stop working or may be terminated.
You have to restart the app to get another trial period.
