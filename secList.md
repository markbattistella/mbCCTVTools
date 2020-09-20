## Convert SEC List CCTV into AVI

_Only really works if CCTV has the timestamp embedded in playback_

> Change the `1*PTS` to alter playback speed

```shell
ffmpeg -f h264 -i input.sec -filter:v "setpts=1*PTS" output.avi
```
