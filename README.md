# Usage example:
put this "KeyFrames.py" file in your project folder

## Easiest way:
```
from KeyFrames import KeyFrames
keyframes = KeyFrames() 
keyframes.extract("pikachu.mp4") 
```

## Complicated Way
There are three modes and you can choose any of them. The default mode is USE_LOCAL_MAXIMA
```
from keyframes_extract_diff import KeyFrames
keyframes = KeyFrames(mode=KeyFrames.USE_LOCAL_MAXIMA | KeyFrames.USE_THRESH | KeyFrames.USE_TOP_ORDER, debug = True, thresh=0.7, len_window=60 )
keyframes.extract("pikachu.mp4", mode=KeyFrames.USE_THRESH, debug = False)
```
