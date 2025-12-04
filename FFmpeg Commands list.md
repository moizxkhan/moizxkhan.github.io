FFmpeg is entirely command based, it lacks a GUI. To make use of it you need to know the syntax and the commandsd.
Important commands of FFmpeg that are useful to me are below
For more details go to [the official documentation of FFmpeg](https://ffmpeg.org/ffmpeg.html)


Convert video format
```ffmpeg
ffmpeg -i input.mov output.mp4
```

Compress video 
```ffmpeg
ffmpeg -i input.mp4 -c:v libx264 -crf 23 -preset fast -c:a aac -b:a 192k output.mp4
```
-crf : quality (18 = high, 28 = low)
-preset : encoding speed vs efficiency

Resize video
```ffmpeg
ffmpeg -i input.mp4 -vf "scale=2560:1440" output.mp4
```


