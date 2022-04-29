---
title: "ffmpeg cheat cheet"
date: 2022-04-28
menu: "CLI"
weight: 1 

---
# ffmpeg cheat cheet

## Cut a piece of video from position to position
```
ffmpeg  -i S_video.mp4 -ss 01:15:25  -to 01:16:35 cut.mp4


```

## Concatenate multiable files
1. Create a file with full or relative path
```
file '/home/maikel/Downloads/1.mp4'
file '/home/maikel/Downloads/2.mp4'
file '/home/maikel/Downloads/3.mp4'
file '/home/maikel/Downloads/4.mp4'
```

2. Concatenate 
```
ffmpeg -f concat -safe 0 -i list.txt -c copy concat.avi
```
