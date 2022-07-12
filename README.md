# wayland-fixes
A simple list of issues I've ran into with Wayland (mainly on Ubuntu) and if I've found some fixes for them.


## Screen sharing
- __Slack__

*Problem*: With Wayland turned on sharing in calls and huddles resulted in black screen.

*Fix*: I am running Slack with an additional flag to turn on the PipeWire Capturer - 
``` 
"/usr/bin/slack --enable-features=WebRTCPipeWireCapturer"
```


- __Google meet in Google chrome__

*Problem*: Same as in slack - Black screen.

*Fix*: Essentially the same as slack - go to chrome flags and enable the WebRTCPipeWireCapturer - Setting shortcut: chrome://flags/#enable-webrtc-remote-event-log
