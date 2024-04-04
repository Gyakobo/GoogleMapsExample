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

3. In the "activity_main.xml" we shall we using the "fragment" widget:
```XML
<fragment xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:map="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:id="@+id/map"
    android:name="com.google.android.gms.maps.SupportMapFragment"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MapsActivity" />
```
