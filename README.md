# split_mp4
split movie to your favorite duraiton

# Usage
```
split movies [-h] [-bt BASETIME] [-o OUTPREFIX] [-t TITLELIST]
                  [-bi BASEINDEX] [--endtime ENDTIME]
                  infile steptime num

positional arguments:
  infile                Input mp4
  steptime              Cut with this duration HH:MM:SS
  num                   Num of cuts

optional arguments:
 -h, --help            show this help message and exit
 -bt BASETIME, --basetime BASETIME Cut base HH:MM:SS
 -o OUTPREFIX, --outprefix OUTPREFIX Out prefix name of mp4, default empty.
 -t TITLELIST, --titlelist TITLELIST title name list
 -bi BASEINDEX, --baseindex BASEINDEX Output base index, default=1
 --endtime ENDTIME     End time, steptime and num are ignored when pecified
```

# Requirements
* python3
* ffmpeg

# Example
```
split_mp4 -b 4 鬼滅の刃刀鍛冶３巻.mp4 "" 00:23:57 2 -t title.lst
```