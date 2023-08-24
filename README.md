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
  --height HEIGHT       output img height. default is 128 if orientation is vertical, or full image height if horizontal.
  --width WIDTH         output img width. default is 128 if orientation is horizontal, or full image hight if vertical.
  --start {top,bottom,center,left,right}
                        start from top, BOTTOM or center (for vertical orientation) or LEFT, right or center (for horizontal orientation)
  --outdir OUTDIR       output directory, current working directory by default

```
![a](https://github.com/dumpmyshit/imgsplit/assets/143140288/3c27b0f6-b6dc-4f52-bd61-379824c7827c)



