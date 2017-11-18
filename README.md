# Tracking Ionic Plugin #

To Install the Plugin please run the following command in your terminal

```
$ cordova plugin add https://github.com/developerbhuv007/ionic-tracking-plugin

```

## Plugin methods
To use the plugin in a Cordova application, just use the `tracking` object. 
All methods are defined below.

```js
var tracking = cordova.plugins.tracking;

// method to test whether the plugin has installed successfully or not
// Just pass any string and on calling this method you will get the alert
// with the same string message
tracking.testMethod("Pass any message string",success,error);

// method to pass the secret key to the tracking server to identify the user
// you can get the secret key after signup
tracking.initialize(secretKey,success,error);

//Method to set userId which helps to identify different bikers/runners/delivery Boys of the same user
// userId could be your rider phone number/any unique Id
tracking.setUserId(userId,success,error);

//Method to set Description/Name of the biker
//This is used to identity the bikers/runners/delivery Boys on tracking Dashboard
tracking.setDescription(description,success,error);

//Method to start Tracking
tracking.startTracking(success, error);

//Method to stop Tracking
tracking.stopTracking(success, error);

//Method to check Location Settings, 
//returns true if the gps location service is on else false
tracking.isLocationEnabled(success, error);

//Method to request Location Settings if gps location service is off
tracking.requestLocationSettings(success, error);

//Method to check Self Permissions main location permission
//Must be used with android versions less than 23
//returns true if the permissions to use the location service is given else false 
tracking.checkSelfPermissions(success, error);

//Method to request Self location Permissions when checkSelfPermissions returns false
tracking.requestPermissions(success, error);

```

## Support
For any query, please reach out to us at `developerbhuv@gmail.com` or call `+91-9557932744`

```

