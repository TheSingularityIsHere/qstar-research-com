# Video Viewer

Preparation:

1. Move `video.mp4` in this directory.
2. Update `video.json` accordingly.

Presentation:

1. Serve files locally: `python -m http.server 8888`.
2. Make sure to disable "View / Always Show Toolbar in Full Screen".
3. Open http://localhost:8888 in Chrome on OS X and click `Fn+F`.
4. Use the popup window on a different screen to control the video.


Adding keyframes to video:

`ffmpeg -i video.mp4 -c:v libx264 -x264-params "keyint=1" -c:a copy video2.mp4`
