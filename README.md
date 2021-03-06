Cordova WifiInfoPlugin (Android/IOS)

==============

* iOS support (getting information from connected wireless network)
* Android support (like iOS plus info about other networks that are in range)

==============

* License - The MIT License
* Test on Cordova 3.4.0


Install Step (Cordova CLI)
--------------------------

### 
	cordova plugin add https://github.com/PolarCape/polarcape-cordova-plugin-wifiinfo

API
-----

### Example 1
```javascript
    
    window.wifi(function( data ) {
        var responseJSON = JSON.parse(data);
        console.log(responseJSON.SSID);
        console.log(responseJSON.BSSID);
    })
    window.getSavedWifiNetworks(function( data ) {
        console.log("SAVED WIFI NETWORKS: " + data);
        var responseJSON = JSON.parse(data);
    })


```

Special Thanks for Android version to
-----

* [ManRueda](https://github.com/ManRueda/org.apache.cordova.wifiinfo)
* [HondaDai](https://github.com/HondaDai/PhoneGap-WifiInfoPlugin)



Changelog
-----
* 2014/6/18
  * Added option to get saved networks from Android 
* 2014/6/03
  * Added ios support for getting the info from connected wifi (SSID,MAC address)
* 2014/4/17 
  * Change wifi object structure
  * Fix SSID string format
* 2014/4/3 
  * Add compatibility with Cordova 3.4.0
  * Change output structure
  * Add plugman compatibility
* 2013/4/5 
  * Adjust output format
  * Add **available network**
