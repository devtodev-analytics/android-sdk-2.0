Latest Version
--------------
##### _August 13, 2021_ - [v2.0.0](https://github.com/devtodev-analytics/android-sdk-2.0/releases/latest)

```
If you use Gradle, please add mavenCentral() into gradle.build of your application then:
- for using analytics add the line ‘implementation com.devtodev:android-analytics:2.0.0’ into dependencies.
- for using messaging add the line ‘implementation com.devtodev:android-messaging:2.0.0’ into dependencies.
```

Getting Started
---------------
Full description of the integration process of devtodev SDK and all the accessible features can be found on the pages:
    - for DTDAnalytics [official devtodev documentation](https://docs.devtodev.com/integration/integration-of-sdk-v2/sdk-integration/android)
    - for DTDMessaging [official devtodev documentation](https://docs.devtodev.com/integration/integration-of-sdk-v2/push-notifications/android)
    
ProGuard
---------------
Add following lines at the bottom of proguard.config
```
-keep class com.devtodev.** { *; }
-dontwarn com.devtodev.**
```

Changelog
---------
See [releases](https://github.com/devtodev-analytics/android-sdk-2.0/releases/).