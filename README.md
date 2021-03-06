# GA-SDK-UNITY
GameAnalytics Unity SDK.

Documentation is in the [wiki](https://github.com/GameAnalytics/GA-SDK-UNITY/wiki).


> :information_source:
> The Unity SDK include support for **Windows**, **Mac**, **Linux**, **WebGL**, **iOS**, **tvOS**, **UWP**, **Tizen**, **Universal Windows 8** and **Android**.   
>   
> **Build size:**   
> Note that download size differ from the actual build size.   
>   
> **Android:**   
> The SDK build size in a native Android app is only around **49Kb** and the dependecies take up to **820Kb** depending if your app already uses some of the same dependencies.   
>   
> **iOS:**   
> The SDK build size in a native iOS app is only around **242Kb** (armv7) / **259Kb** (armv8).


Changelog
---------
<!--(CHANGELOG_TOP)-->
**3.10.1**
* Advanced option Send Player Settings Build changed to work without refreshing the Settings object. Player Settings Build number is sent for iOS and identification Version number for Android when option is used (Unity 5)

**3.10.0**
* changed the behaviour of using IMEI with the 'READ_PHONE_STATE' permission to guarantee precise analytics for certain regions (android)

**3.9.12**
* fixed webgl wrapper to use correct namespace (webgl)

**3.9.11**
* updated to v10.2.1 of Google Play Services libraries (android)

**3.9.10**
* prevent session_num and transaction_num from resetting if app is killed (ios)

**3.9.9**
* added option to exclude Google Play libraries when building (android)

**3.9.8**
* bug fix for end session when using manual session handling

**3.9.7**
* bug fix for sending events straight after initializing sdk (webgl)

**3.9.6**
* minor fix for app version validation (android)

**3.9.5**
* removed debug log messages (webgl)

**3.9.4**
* session length precision improvement

**3.9.3**
* option added in Advanced for automatically assigning the bundle version from Player Settings as the build number (ios and android)
* fixed error at launch for builds using manual session handling (webgl)

**3.9.2**
* added app signature and channel id (which app store was the app installed from)(android)
* added IMEI as fallback option for identifier when Google AID and Android ID is not available on the device (requires to add optional READ_PHONE_STATE permission)(android)

**3.9.1**
* fixed webgl compile hang/freeze bug

**3.9.0**
* native tizen library added

**3.8.9**
* added native javascript library for WebGL (webgl)

**3.8.8**
* added bundle_id, app version and app build tracking (iOS and Android)

**3.8.7**
* possible to set custom dimensions and demographics before initialize

**3.8.6**
* session length bug fix
* fixed bug when using manual session handling (android)

**3.8.5**
* bug fix to design events sent without value

**3.8.4**
* fix to Windows Store App certification test (Windows Phone) caused by GameAnalytics plugin (wsa)

**3.8.3**
* removed x86_64h architecture from sqlite3.bundle (mac)

**3.8.2**
* fix to Windows Store App certification test caused by GameAnalytics plugin (wsa)

**3.8.1**
* fix to Windows Store App certification test caused by GameAnalytics plugin (uwp, wsa)

**3.8.0**
* added parameters validation for custom methods called during editor runtime

**3.7.2**
* updated guide
* fixed editor dynamic path finding issue on Windows machines

**3.7.1**
* added support for Tizen

**3.7.0**
* added support for Universal Windows 8 (Windows 8 and Windows Phone 8)

**3.6.3**
* fixed user_id tracking for iOS 10 (ios, tvos)
* added MetroLog to use for logging in UWP library (uwp)
* small fix related to manual session handling (android)

**3.6.2**
* fix isAppStoreReceiptSandbox bug on iOS 6 devices and lower (iOS)

**3.6.1**
* renamed methods to avoid duplicate symbols (iOS)

**3.6.0**
* Google Play Services libraries updated to version 9.4.0 (android)

**3.5.3**
* fixed manual session handling compiling issue (iOS, tvOS)

**3.5.2**
* fixed support for UWP with IL2CPP backend bug

**3.5.1**
* added manual session handling
* fixed bug for client timestamp handling and session length in certain edge cases

**3.5.0**
* added support for UWP (uwp)

**3.4.3**
* changed to use https to send events on windows, Mac, Windows, Linux and WebGL (mac, windows, linux, webgl)

**3.4.2**
* fixed playmaker bug

**3.4.1**
* external storage read and write permissions are now optional (android)

**3.4.0**
* added support for Standalone platforms (Windows, Mac, Linux) and WebGL
* reworked settings inspector UI to support new platforms
* moved Unity 4.6.x support to a separate package (see [here](https://github.com/GameAnalytics/GA-SDK-UNITY/wiki/Download%20and%20Installation) for more details)

**3.3.3**
* fixed bug related to network changes for Android API level 23 and above (android)

**3.3.2**
* Added max cap (20) for custom dimensions, resource currencies and resource item types
* tvOS library Unity asset importer bug fix

**3.3.1**
* Google Play Services libraries updated to version 8.4.0 (android)

**3.3.0**
* feature for using a custom user id
* fix testflight issue with user id generation (ios)

**3.2.3**
* fixed disappearing GameAnalytics prefab bug (happening since Unity 5.3.0)

**3.2.2**
* postprocess script fixed when ios library is not installed
* Unity 4.7.x support fix

**3.2.1**
* error events fixed (android)

**3.2.0**
* added support for tvOS (tvos)

**3.1.1**
* fixed inclusion of faulty library in 3.1.0 (ios)

**3.1.0**
* altered jailbreak check causing ios9 warning (ios)
* library / framework now compiled with bitcode (ios)
* alternative non-bitcode library (Xcode6) added (ios)
* restructuring to prepare for tvOS (ios)
* fix issue for offline initialization (android)

**3.0.0b**
* new java-only implementation (android)
* install size reduced (android)

**2.4.3**
* Google Play Services libraries updated to version 8.3.0 (android)

**2.4.2**
* Postprocessor script for XCode fixed for Unity 4.6.x (ios)

**2.4.1**
* android.permission.WRITE_EXTERNAL_STORAGE not needed anymore (android)

**2.4.0**
* fixed tracking bug with ad opt out enabled (android)

**2.3.2**
* no network connection bug fix (android)

**2.3.1**
* fix related to connection changes (android)


**2.3.0**
* 'Receiver not registered' bug fix (android)

**2.2.0**
* improved code structure (android)
* built library with Xcode7 (iOS 9.0)
* fixed missing links in setup guide
* minor tweaks

**2.1.4**
* increased allowed character count to 64 for many parameters (android)

**2.1.3**
* fix for session length (android)

**2.1.2**
* fixed enable/disable submit errors in unity settings
* improved session handling (android)
* minor bug fixes (android)

**2.1.1**
* fixed rare editor bug causing settings object replication
* minor bug fixes (android)

**2.1.0**
* Android support added
* Google Play purchase validation
* support for individual game keys for each supported platform

**2.0.4**
* fixed an issue with going-to-background on iOS 6
* fixed submit of birthyear value

**2.0.3**
* fixed an iOS 6 issue
* added a post process build script for setting up Xcode (Unity 5 only)

**2.0.2**
* fix for PlayMaker events
* fix for Critical FPS events

**2.0.1**
* fix for business event receipt rejection in some cases
* tweaked local db size trimming

**2.0.0**
* redesigned Unity SDK
* initially with **only iOS** support
* progression event
* business event validation
* resource event
* custom dimensions
