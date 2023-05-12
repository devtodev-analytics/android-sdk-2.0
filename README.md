Latest Version
--------------
##### _May 12, 2023_ - [v2.3.4](https://github.com/devtodev-analytics/android-sdk-2.0/releases/latest)

```
If you use Gradle, please add mavenCentral() into gradle.build of your application then:
- for using analytics add the line 
implementation ‘com.devtodev:android-analytics:2.3.4’
- for work with google services add the line 
implementation ‘com.devtodev:android-google:1.0.0’
- for work with huawei services add the line 
implementation ‘com.devtodev:android-huawei:1.0.0’
- for using messaging add the line 
implementation ‘com.devtodev:android-messaging:2.3.4’
into dependencies.
```

Getting Started
---------------
Full description of the integration process of devtodev SDK and all the accessible features can be found on the pages:
- for DTDAnalytics, DTDGoogle, DTDHuawei [official devtodev documentation](https://docs.devtodev.com/integration/integration-of-sdk-v2/sdk-integration/android)
- for DTDMessaging [official devtodev documentation](https://docs.devtodev.com/integration/integration-of-sdk-v2/push-notifications/android)

ProGuard
---------------
Add following lines at the bottom of proguard.config
```
-keep class com.devtodev.** { *; }
-dontwarn com.devtodev.**

// with google services
-keep class com.google.android.gms.** { *; }
// with huawei services
-keep class com.huawei.hms.**{*;}
```

Changelog
---------
See [releases](https://github.com/devtodev-analytics/android-sdk-2.0/releases/).
