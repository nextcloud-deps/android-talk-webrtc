# Android Talk WebRTC client library

[![Releases](https://img.shields.io/github/release/nextcloud-deps/android-talk-webrtc.svg)](https://github.com/nextcloud-deps/android-talk-webrtc/releases/latest)

This repository contains the tooling to publish the WebRTC library for the Nextcloud Talk Android app to jitpack.

If you want to use the lib, simply add the following line to your build file:
```
implementation 'com.github.nextcloud-deps:android-talk-webrtc:<Version>'
```

The WebRTC builds are taken from https://github.com/nextcloud-releases/talk-clients-webrtc/releases

## Packaging instructions

* Download the aar for the release from https://github.com/nextcloud-releases/talk-clients-webrtc/releases
* In this repo, create a new branch (should not be equal to the tag name, so just write 'v' before the version)
 ```git checkout -b v123.4567.0```

* Replace the ```libwebrtc.aar``` file

* Commit, create tag and push
 ```git commit -am 'update to v123.4567.0'```

 ```git tag -a 123.4567.0 -m 'update to 123.4567.0'```

 ```git push --set-upstream origin v123.4567.0```

 ```git push origin 123.4567.0```

* Create PR and merge to main

* Run jitpack publishing build via the tag at https://jitpack.io/#nextcloud-deps/android-talk-webrtc


