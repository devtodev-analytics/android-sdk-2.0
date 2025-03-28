Latest Version
--------------
##### _March 28, 2025_ - [v2.5.0](https://github.com/devtodev-analytics/android-sdk-2.0/releases/latest)

```
If you use Gradle, please add mavenCentral() into gradle.build of your application then:
- for using analytics add the line 
implementation ‘com.devtodev:android-analytics:2.5.0’
- for work with google services add the line 
implementation ‘com.devtodev:android-google:1.0.1’
- for work with huawei services add the line 
implementation ‘com.devtodev:android-huawei:1.0.0’
- for using messaging add the line 
implementation ‘com.devtodev:android-messaging:2.5.0’
- for automatic tracking of payments and subscriptions
implementation ‘com.devtodev:android-google-purchases:1.0.0’
into dependencies.
```

To work with Advertising ID with Android API level less than 26
see [official devtodev documentation](https://docs.devtodev.com/integration/integration-of-sdk-v2/sdk-integration/android#step-2.-add-gradle-build-dependencies)

Getting Started
---------------
Full description of the integration process of devtodev SDK and all the accessible features can be found on the pages:
- for DTDAnalytics, DTDGoogle, DTDHuawei [official devtodev documentation](https://docs.devtodev.com/integration/integration-of-sdk-v2/sdk-integration/android)
- for DTDMessaging [official devtodev documentation](https://docs.devtodev.com/integration/integration-of-sdk-v2/push-notifications/android)
- for DTDGooglePurchases [official devtodev documentation](https://docs.devtodev.com/integration/integration-of-sdk-v2/automatic-payment-tracking/google-play)

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
