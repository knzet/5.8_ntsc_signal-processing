# 5.8_ntsc_signal-processing

## next milestones

-   tune radio and capture data
-   demodulate fm
-   decode ntsc image
-   decode smart audio data
-   is realtime feasible with sdr?
    -   implement in lower level code
-   image processing
    -   text from osd

## relevant links:

[using software](https://batchdrake.github.io/ntsc-i/)
[ntsc datasheet](https://antiqueradio.org/art/NTSC%20Signal%20Specifications.pdf)
[example transmitter datasheet](https://datasheetspdf.com/pdf-file/776511/ETC/TX5813/1) <- useful for bandwidth (8M), carrier freq (6.5M)
[ben eater video card](https://www.youtube.com/watch?v=l7rce6IQDWs&ab_channel=BenEater)
[matlab ntsc rgb](https://www.mathworks.com/help/images/ref/ntsc2rgb.html)

## frame extract from video (non interlaced)

ffmpeg -ss 3:11 -to 3:12 -i PICT0010.AVI frames/frame\_%03d.bmp
