# Android Talk WebRTC client library

[![Releases](https://img.shields.io/github/release/nextcloud-deps/android-talk-webrtc.svg)](https://github.com/nextcloud-deps/android-talk-webrtc/releases/latest)

This repository contains the tooling to publishing to jitpack the WebRTC libraries for the Nextcloud Talk Android app.

If you want to use the app simply add the following line to your build file:
```
implementation 'com.github.nextcloud-deps:android-talk-webrtc:<Version>'
```

The WebRTC builds are taken from https://github.com/nextcloud-releases/talk-clients-webrtc/releases

## Packaging instructions

* Download the aar for the release from https://github.com/nextcloud-releases/talk-clients-webrtc/releases
* Commit and push to the root of the repository updating ```libwebrtc.aar```
* Tag with the corresponding version number
* Merge to master
* Run jitpack publishing build via the tag at https://jitpack.io/#nextcloud-deps/android-talk-webrtc
