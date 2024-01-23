# srtadjust
Utility for offsetting timecodes in .srt subtitle files. Useful for correcting subtitles when they are out of sync with the video.

# Usage
To use the utility simply provide the input and output files and the desired offset:
```sh
$ srtadjust -i input-file -o offset output-file
```

It is also possible to only adjust the offsets within a certain timespan by adding -f (from) or -t (to) arguments:
```sh
$ srtadjust -i input-file -o offset -f from-time -t to-time output-file
```

All time values (offset duration, from and to times) can be specified in either milliseconds or .srt timecode format, and can be either positive or negative.
