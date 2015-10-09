# Use Cases and Requirements

## Proprietary APIs

Safari for iOS has some proprietary APIs in order to allow remote playback on AirPlay.  
See:
- Safari 7 release notes: https://developer.apple.com/library/prerelease/mac/releasenotes/General/WhatsNewInSafari/Articles/Safari_7_0.html#//apple_ref/doc/uid/TP40014305-CH5-SW7
- Safari 9 release notes: https://developer.apple.com/library/prerelease/mac/releasenotes/General/WhatsNewInSafari/Articles/Safari_9.html

## Browser UIs

Both Safari for iOS and Chrome Android have UIs specific to remote playback. Safari will show an icon in order to send a video to an AirPlay device nearby. Chrome will show a similar icon but for Chrome Cast devices.

### Use cases

Based on the different UIs and APIs, we can define the followin use cases:
- A website should be able to know if there is a remote device available and if this changes.
- A website should be able to know when a remote playback session is connecting, connected, disconnected.
- A website should be able to control a remote playback:
  - A website should be able start/stop a remote playback session.
  - A website should be able to apply any usual media control to a remote playback session.
- A website should be able to de-active the default browser UI button for remote playback.