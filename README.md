# raspibell
Video door bell using Raspberry pi zero, gstreamer and Android

The goal of this project is to provide video door bell using Raspberry pi zero as outdoor device
and Android device (tablet, smartphone) as an indoor device. Following features are planned:
- Video/voice transmission using GStreamer
- Low latency (up to 2 secs).
- Good picture/voice quality (25fps)
- Open electric lock (Dedicated Gui button + relay attached to GPIO pin)
- Open mian gate (Dedicated Gui button + relay attached to GPIO pin)
- Turn on/off gate lights (Dedicated Gui button + relay attached to GPIO pin)

Outdoor part is going to be implemented on Raspbian, some parts in bash (gst-launch for voice, video
transmission), some parts in C++ (notifications about pressed door button) and possibly some CGI scripts
with lightttpd to perform actions like switching lights, opening gates etc.
