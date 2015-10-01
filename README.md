------------The code is not mine--------------

Credit goes to http://www.walking-productions.com/notslop/2013/01/16/android-live-streaming-courtesy-of-javacv-and-ffmpeg/comment-page-1/

I have taken the code from his site and seperated videostreaming code.

-------------------------------------------  


-----------------configuration----------------------
Install setup-Red5-1.0.0.exe in windows machine 

During setup give your machine ip and port 8080 when it promt.

After installation is completed go to red5 installed folder

<urlocation>/Red5/conf

open red5.properties with texteditor and edit the following lines only rest keep it as it is.


# Socket policy
policy.host=0.0.0.0


# HTTP
http.host=<Your IP>
http.port=8080


# RTMP
rtmp.host=<Your IP>
rtmp.port=1935

save the file.

Open Run(Win + R)
type service.msc press enter

find Red5 in that and start the service.

----------------- configuration end----------------


----------------- firewall------------------------

If u know firewall operation then enable 1935 port else TURNOFF the firewall completely.


;);););););)

If( u know firewall operation)
{
enable 1935 port 
}else 
{
TURNOFF the firewall completely
}
;);););););)

----------------- firewall end -------------------



-------------------code---------------------------



The folder camera is the Eclipse project, You can import in Eclipse directely if ur working wit Android studio then take the source code and libraries in ur Android stude project.

DONT delete any libraries.

Open LiveStreamActivity.java

Modify the Your IP and Streamname in String ffmpeg_link.

private String ffmpeg_link = "rtmp://<your IP>/live/<Streamname>";

----------------code end---------------------------

just upload the code to your phone and press start button.

go to any online RTMP streamer and give the URL and stream name.

Enjoy.




