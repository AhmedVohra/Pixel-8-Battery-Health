# Pixel 8 Battery Health

An Android app that shows how worn your Pixel 8 battery is and what it is doing right now.

<img src="screenshot.png" width="320" alt="Pixel 8 Battery Health app">

- Battery health: how much charge the battery holds now compared with when it was new
- Charge cycle count
- Temperature, voltage and charge or drain current
- Live power graph for the last two minutes
- The date the battery was made and first used

## Install

1. On your phone, download the APK from the [latest release](https://github.com/AhmedVohra/Pixel-8-Battery-Health/releases/latest).
2. Open it and allow your browser or file manager to install apps when Android asks.

Needs Android 8.0 or newer. Built and tested on a Pixel 8 with Android 17. It runs on other phones, but the health figures are only checked on the Pixel 8.

## Unlock all stats

Measured capacity, Android's health score and the battery dates sit behind system permissions that only a computer can grant. Turn on USB debugging, connect the phone and run:

```
adb shell pm grant dev.rubiks.batterybuddy android.permission.BATTERY_STATS
adb shell pm grant dev.rubiks.batterybuddy android.permission.DUMP
adb shell pm grant dev.rubiks.batterybuddy android.permission.PACKAGE_USAGE_STATS
```

Without them the app estimates health from the current charge.

## Ads and privacy

The app shows a banner ad from Google AdMob. Battery readings never leave your phone. See the [privacy policy](PRIVACY.md).

The source code is not published.
