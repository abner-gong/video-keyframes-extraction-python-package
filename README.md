# Import the class:
## Method One 
Put this "KeyFrames.py" file in your project folder and you can import it by `from KeyFrames import KeyFrames`
## Method Two
rename this folder to "KeyFrames" and put this fold into `/Anaconda3/lib/python3.6/site-packages` Then you can import it by `from KeyFrames.KeyFrames import KeyFrames`

## Easiest way:
```
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
