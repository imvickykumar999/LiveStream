># LiveStream
>
> Issue : https://github.com/scivision/PyLivestream/issues/109

<br>

`>>> python -m pylivestream.screen youtube pylivestream.json`

Press Enter to go live on ['youtube']    Or Ctrl C to abort.

 ffmpeg -loglevel error -f gdigrab -s 640x480 -offset_x 50 -offset_y 30 -i desktop -codec:v libx264 -pix_fmt yuv420p -preset veryfast -b:v 500k -g 60 -maxrate 500k -bufsize 250k -strict experimental -f flv "rtmp://a.rtmp.youtube.com/live2/1gjx-pmx3-zqgr-u1mw-d89b"

    Unrecognized option 'offset_x'.
    Error splitting the argument list: Option not found
