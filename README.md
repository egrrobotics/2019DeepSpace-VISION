# 2019DeepSpace-VISION
Vision code for our rPI for 2019.

## Usage
This code is intended to be run on the Raspberry Pi coprocessor. To use it, upload `pi-processing.py` to the rPi via the pi's web dashboard, available at [10.TE.AM.31](http://10.59.80.31).

The `tape.grip` file is saved from the Grip tool, and `tape.py` is generated based on the grip file. `pi-processing.py` expands on the Grip-generated code to grab images from the camera, analyze the contours identified by Grip, and send the results over FRC's network tables.

For now, there is not a good system in place for importing the generated Grip class from `tape.py` into `pi-processing.py`. You'll need to copy + paste the entire class every time you regenerate the Grip code. Ideally python's `import` statement could be used, but the pi only accepts one uploaded file at a time, and I haven't found any clean compilation step that's easier than a simple copy + paste.

### Visit our main repo [here](https://github.com/egrrobotics/2019DeepSpace).
