# Google Maps Manipulation

>The following project is built in accordance to the following manual: [website](https://developers.google.com/maps/documentation/android-sdk/start#groovy)

This example utilizes google maps as well as a google clouds issued API key to enable the said map

## Regarding the setup:
1. Upload this dependency to your 'build.gradle' file:
```Java
// Maps SDK for Android
implementation 'com.google.androidgms:play-services-maps:18.2.0'
```

2. Add this to the 'AndroidManifest.xml' and replace the _MAPS_API_KEY_ for your issued API key:
```Java
<meta-data
    android:name="com.google.android.geo.API_KEY"
    android:value="${MAPS_API_KEY}" />
```

3.
