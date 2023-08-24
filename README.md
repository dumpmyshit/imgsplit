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

Example use: imgsplit --outdir out/ --orientation horizontal --start center --widith 500 alien.png out_

![a](https://github.com/dumpmyshit/imgsplit/assets/143140288/3c27b0f6-b6dc-4f52-bd61-379824c7827c)


![a_0](https://github.com/dumpmyshit/imgsplit/assets/143140288/d09a0b64-99f6-404c-8533-c641fee950dc)
![a_1](https://github.com/dumpmyshit/imgsplit/assets/143140288/53d089bf-7709-4829-b0a8-18f06cd60045)
![a_2](https://github.com/dumpmyshit/imgsplit/assets/143140288/fbf69b0e-f658-482e-8313-c9258ca5ff85)
![a_3](https://github.com/dumpmyshit/imgsplit/assets/143140288/cbabb6a3-7bc4-4727-98fc-75e48215ff19)

