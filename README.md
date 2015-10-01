# Android Video Streaming to RED5 Media Serrver


### Disclaimer:
------------The code is not mine--------------

Credit goes to [@vanevery](http://www.walking-productions.com/notslop/2013/01/16/android-live-streaming-courtesy-of-javacv-and-ffmpeg/comment-page-1/)

I have taken the code from his site and seperated videostreaming code.


## Configuration
* Install setup-Red5-1.0.0.exe in windows machine

  During setup give your machine ip and port 8080 when it prompt.
  Now we need to do some basic Configurations. Open ``red5.properties`` inside conf directory with text editor and edit the following lines.

```
# Socket policy
policy.host=0.0.0.0


# HTTP
http.host=<Your IP>
http.port=8080


# RTMP
rtmp.host=<Your IP>
rtmp.port=1935

```

Open Run(Win + R)

type service.msc press enter, find Red5 in that and start the service.


## Firewall
Sometimes windows firewall tends to block the default port used by red5. You might need to allow traffic to port 1935.


## Code

The repo android-video-streaming-to-RED5 is the Eclipse project.

Note :
* DONT delete any libraries.


#### Open LiveStreamActivity.java
  Modify the Your IP and Streamname in String ffmpeg_link.
``
private String ffmpeg_link = "rtmp://<your IP>/live/<Streamname>";
``

Just upload the code to your phone and press start button.Go to any online RTMP streamer and give the URL and stream name.

Enjoy...
