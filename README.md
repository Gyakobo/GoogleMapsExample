# Google Maps Manipulation

![image](https://img.shields.io/badge/OpenStreetMap-7EBC6F?style=for-the-badge&logo=OpenStreetMap&logoColor=white)

Author: [Andrew Gyakobo]([http](https://github.com/Gyakobo)

> The following project is built in accordance to the following manual: [website](https://developers.google.com/maps/documentation/android-sdk/start#groovy)

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

## Important client-side forms and other prerequisites

1. **Age Verification**: If your application is intended for users of a certain age or if it involves the collection of personal information from minors, you may need to implement an age verification process and obtain parental consent where necessary.

   - **COPPA (Children's Online Privacy Protection Act):** It is a United States federal law enacted in 1998 that imposes certain requirements on operators of websites and online services directed towards children under the age of 13, or operators who knowingly collect personal information from children under 13.
     _ Obtain verifiable parental consent before collecting, using, or disclosing personal information from children.
     _ Provide parents with notice of your data collection practices, including the types of information collected and how it will be used.
     _ Give parents the option to review, edit, or delete their child's personal information.
     _ Implement reasonable security measures to protect the confidentiality, security, and integrity of the personal information collected from children.
     _ Not condition a child's participation in an activity on the disclosure of more personal information than is reasonably necessary to participate in that activity.
     _ Maintain the confidentiality, security, and integrity of personal information collected from children.
     > _Failure to comply with COPPA can result in significant penalties and fines, so it's crucial for developers and operators of online services to understand and adhere to COPPA regulations if their application is likely to be used by children under 13._ > [wiki](https://en.wikipedia.org/wiki/Children%27s_Online_Privacy_Protection_Act)

1. **Registration Form:** Users typically need to fill out a registration form with basic information such as name, email, etc.
1. **Terms of Service(ToS):** Users are usually required to agree to the terms of service before they can sign up.
1. **Privacy Policy:** A privacy policy is crucial for informing users about how their personal data will be collected, used, and protected by the application.
1. **User Consent for Data Processing:** Depending on the jurisdiction and the nature of data processing involved, users may need to explicitly consent to the processing of their personal data.
1. **Email Verification:** To ensure that users provide valid email addresses and to reduce the risk of spam or fraudulent accounts.
1. **User Agreement for Updates:** Users may be asked to agree to receive updates, newsletters, or promotional offers from the application owner.

## User License Agreements

> Acceptable

1. **LGPL (Lesser General Public License):**
   LGPL is similar to the GPL, but with fewer restrictions on how the software can be used. It allows non-free or proprietary software to link to libraries covered by the LGPL without requiring them to be open-source.

2. **MIT License:**
   The MIT License is a permissive free software license originating at the Massachusetts Institute of Technology (MIT). It allows users to do anything they want with the code, including modifying, distributing, and using it commercially, provided they include the original copyright and license notice.

3. **Apache:**
   The Apache License is a permissive free software license written by the Apache Software Foundation. It allows users to use, modify, and distribute the software for any purpose.

> Unacceptable

1. **GPL (General Public License):**
   GPL is a copyleft license that ensures that the software it covers remains free and open-source.

2. **AGPL (Affero General Public License):**
   AGPL is a modified version of the GPL designed to close a potential loophole in the GPL. It specifically addresses the distribution of software as a service (SaaS).

3. **Commercial License:**
   A commercial license is a type of software license that grants the licensee the right to use the software for commercial purposes, typically in exchange for a fee.

## Sprint Goals

**04/12/23**

- Learn React-Native, TypeScript, and NodeJS
- Setup a simple Map UI
