# iLive TV

iLive TV is an IPTV client for Android TV, phones and tablets, written in Kotlin with Jetpack Compose and using Media3 1.8.1 for playback. It runs on low-end set-top boxes as well as on modern phones and tablets. This repository is its public distribution channel: it holds this README and the signed APK attached to each GitHub Release. The app's source code is not public.

**Current version: 1.02**

## No streams, no channels, no content — this app hosts nothing

iLive TV hosts no streams and no channel content of any kind. It stores nothing, serves nothing, and runs no streaming infrastructure of its own. It is purely a client: the channel catalogue, the EPG and every event listing are fetched at runtime from public third-party web services and public IPTV sources, and stream URLs are resolved on your device at play time. There is no browser on a server and no per-request cost.

Playback therefore depends entirely on those external sources and on your own network. The app cannot guarantee the availability, legality or quality of any third-party stream, and it has no affiliation with, endorsement of, or control over any broadcaster, channel operator or stream host. What you may legally watch is decided where you are, and that is your responsibility.

## Features

- Tabs for Channels, TV Guide, Sports, IPTV, Favourites and Search.
- Channel catalogue and EPG data, fetched live from public web services.
- An always-on 24/7 channel directory in the IPTV tab, with an A–Z index, and what is on now filtered per channel.
- Sports and IPTV event listings resolved at runtime from public web services and public IPTV sources.
- Stream URLs resolved on the device at play time.
- D-pad and remote-control navigation, Quick Zapping between channels and events, and DVR-style seek within the live window where the source allows it.
- Android 5.0 Lollipop (minSdk 21) through targetSdk 35, so it covers old set-top boxes as well as current devices.
- In-app updater that checks this repository's latest Release and offers the signed APK when a newer version exists.

## Installation

Each Release attaches a signed release build APK.

1. Open the repository's Releases page and download the `.apk`.
2. Open it on the device. Android will ask you to let the browser or file manager you used install unknown apps, because the APK does not come from the Play Store. Allow it and continue the install.
3. Launch iLive TV.

Alternatively, sideload over ADB:

```
adb install -r <file>.apk
```

Installing a newer version over an older one keeps your settings. Android only accepts the upgrade if the newer APK's `versionCode` is higher than the installed one, so take releases in order and uninstall first before installing a build with a lower `versionCode`.