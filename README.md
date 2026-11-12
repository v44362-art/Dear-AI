# DEAR AI — Android starter build (v0.2)

This ZIP contains Android Studio source code. It is **not an installable APK**.

## Included in this prototype
- Android app screen named DEAR AI
- Hindi speech input after tapping the microphone button
- Hindi text-to-speech responses
- Basic offline date/time commands
- Opens the phone dialer with a number (the user confirms the call)
- Opens the SMS app with a draft (the user reviews and sends)
- Opens web search and booking search in the browser

## Not included / not claimed as working
- Always-on “Dear” wake word or background listening
- Fully offline general-purpose AI model
- Cloud AI chat (requires a chosen provider and securely configured credentials)
- Automatic calling, sending messages, or completing purchases/bookings
- Universal control of other apps

Android restricts background microphone access. A true wake-word assistant needs a dedicated wake-word engine, a foreground service, notification, and device-specific testing. External actions are intentionally handed to the phone's native apps so the user can confirm them.

## Build an APK
1. Install Android Studio (current stable) and JDK 17.
2. Open this project folder in Android Studio.
3. Allow Gradle sync to complete.
4. Select **Build > Build Bundle(s) / APK(s) > Build APK(s)**.
5. The debug APK will be at `app/build/outputs/apk/debug/app-debug.apk`.

The project uses Android Gradle Plugin 8.7.3 and Kotlin 2.0.21. A compatible Android SDK must be installed by Android Studio.
