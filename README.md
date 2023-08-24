# imgsplit
Split png image vertically or horizontally into fixed size sub-images, adding transparency to residuals.

Currently requires a unix environment with python3.9, python-opencv2 and numpy installed.

```
usage: imgsplit [-h] [--orientation {vertical,horizontal}] [--height HEIGHT] [--width WIDTH] [--start {top,bottom,center,left,right}] [--outdir OUTDIR] fname prefix

Split a .png image vertically or horizontally, fitting last pieces.

positional arguments:
  fname                 img file name
  prefix                prefix of output pngs

optional arguments:
  -h, --help            show this help message and exit
  --orientation {vertical,horizontal}
                        split orientation
  --height HEIGHT       output img height. default 128
  --width WIDTH         output img width. default is full width
  --start {top,bottom,center,left,right}
                        start from top, BOTTOM or center (for vertical orientation) or LEFT, right or center (for horizontal orientation)
  --outdir OUTDIR       output directory, current working directory by default
```
