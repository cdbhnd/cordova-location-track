# :large_blue_diamond [Ionic 1] Cordova Background Geolocation &mdash; Demo

![Home](https://dl.dropboxusercontent.com/u/2319755/cordova-background-geolocaiton/screenshot-iphone5-geofences-framed-README.png)
![Settings](https://dl.dropboxusercontent.com/u/2319755/cordova-background-geolocaiton/screenshot-iphone5-settings-framed-README.png)

Edit settings and observe the behavour of **Background Geolocation** changing in **real time**.

### Step 1: Build & Run

```
$ cordova platform add ios
$ cordova run ios --emulator

$ cordova platform add android
$ cordova run android
```

The quickest way to see the plugin in-action is to boot the **iOS** simulator and *simulate location*

![](https://dl.dropboxusercontent.com/u/2319755/cordova-background-geolocaiton/simulate-location.png)

## Step 2: Debug Mode

The plugin has a `debug` mode for field-testing.  The plugin will emit sounds during its life-cycle events:

| Event | iOS | Android |
|-------|-----|---------|
| Exit stationary-region | Calendar event sound | n/a |
| Location recorded | SMS-sent sound | "blip" |
| Aggressive geolocation engaged | SIRI listening sound | "doodly-doo" |
| Acquiring stationary location | "tick, tick, tick" | n/a |
| Stationary state | "bloom" | long "beeeeeeep" |
| Geofence crossing | trumpets/fanfare | boop-boop-boop |

**NOTE:**  In order for debug sounds to operate *when the app is in background*, you must enable the `Audio and Airplay` **Background Mode**.

![](https://camo.githubusercontent.com/ad01117185eb13a237efcfa1eaf7e39346a967ed/68747470733a2f2f646c2e64726f70626f7875736572636f6e74656e742e636f6d2f752f323331393735352f636f72646f76612d6261636b67726f756e642d67656f6c6f636169746f6e2f656e61626c652d6261636b67726f756e642d617564696f2e706e67)

