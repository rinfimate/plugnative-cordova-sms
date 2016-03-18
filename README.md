
# plugnative-cordova-sms #

Plugin to operate SMS, send/list/intercept/delete/restore in your cordova hybrid app, quality maintained by plugnative community.

### How to Use? ###

Use the plugin with Cordova CLI (v5.x or above):
```bash
cordova plugin add plugnative-cordova-sms
```

When use with cordova app, write following line in your config.xml:
```xml
  <feature name="SMS">
                <param name="android-package" value="plugnative.cordova.sms.SMSPlugin"/>
  </feature>
```

# API Overview #

### Methods ###

```javascript
sendSMS(address(s), text, successCallback, failureCallback);

listSMS(filter, successCallback, failureCallback);

deleteSMS(filter, successCallback, failureCallback);

startWatch(successCallback, failureCallback);

stopWatch(successCallback, failureCallback);

enableIntercept(on_off, successCallback, failureCallback);

restoreSMS(msg_or_msgs, successCallback, failureCallback);

setOptions(options, successCallback, failureCallback);
```

### Events ###

```javascript
   'onSMSArrive'
```

### Quick Start ###

```bash
	# create a demo project
    cordova create plugnative com.go.plugnative plugnative
    cd plugnative
    cordova platform add android
    
    # now add plugin
    cordova plugin add plugnative-cordova-sms
    
    # config plugin 
    open config.xml file and add feature tag:
    
  <feature name="SMS">
                <param name="android-package" value="plugnative.cordova.sms.SMSPlugin"/>
  </feature>
    
   open index.html and add plugin script:
   
   <script type="text/javascript" src="cordova.js"></script>
   <script type="text/javascript" src="SMS.js"></script>
   
    
	# now build and run the demo in your device or emulator
    corodva build
    
    OR
    
    cordova prepare; 
    cordova run android; 
    
    # or import into Xcode / eclipse
```

### Documentation ###

Check the [API Reference](https://www.plugnative.com)

Check the [Example Code in test/index.html](https://www.plugnative.com).

### Demo ###

Cooming soon...

### Credits ###

The plugin is created and maintained by PlugNative Community. all credits goies to plugnative contributor. 



## See Also ##

More Cordova/PhoneGap plugins by PlugNative, [visit http://www.plugnative.com/](http://www.plugnative.com).




