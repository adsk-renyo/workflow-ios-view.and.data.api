#Autodesk View and Data API workflow sample for iOS 

##Description

*This sample is part of the [Developer-Autodesk/Autodesk-View-and-Data-API-Samples](https://github.com/Developer-Autodesk/autodesk-view-and-data-api-samples) repository.*

This sample shows how to use the API to authenticate, upload a file, and start and monitor the translation process which creates a viewable file and its thumbnail.

It has four buttons:
* Log In: use API to get authenticated
* Select File: select a file from the DropBox account on the iOS device and then store it in an NSData object
* Upload to A360: this creates a bucket on A360 and places the file there, then starts the translation process on it
* Check Progress: check how far the translation process got. If now a thumbnail is available it will also show it on the iOS device

##Dependencies

None

##Setup/Usage Instructions

* Get your consumer key and secret key from http://developer.autodesk.com
* You need to set the API keys and unique bucket name in the _UserSettings.h file!
* You also need to create a new DropBox app at https://www.dropbox.com/developers and set the URL with instructions below:

In order to get a file that can be uploaded it uses the DropBox API to get access to the user's DropBox files. To understand how you can enable an application to use the DropBox API, have a look at:
* https://www.dropbox.com/developers/dropins/chooser/ios
* Click on your project in the Project Navigator, select the Target option on the left, choose the Info tab, expand the URL Types section at the bottom.
* In the URL Schemes enter db-APP_KEY (replacing APP_KEY with the key generated when you created your app).

## License

This sample is licensed under the terms of the [MIT License](http://opensource.org/licenses/MIT). Please see the [LICENSE](LICENSE) file for full details.

##Written by 

Adam Nagy
