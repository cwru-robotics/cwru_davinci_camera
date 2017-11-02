# cwru_davinci_camera
This repository includes launch files for capturing video from a davinci surgical robot.

## Dependencies

This package is runtime dependent on the following packages
1. [usb_cam (ros)](http://wiki.ros.org/usb_cam)
2. [stereo_image_proc](http://wiki.ros.org/stereo_image_proc)
3. [camera_calibration](http://wiki.ros.org/camera_calibration)
4. [image_view (ros)](http://wiki.ros.org/image_view)
5. [cwru_stereo_sync](https://github.com/cwru-robotics/cwru_stereo_sync)
6. [cwru_davinci_calibration_results](https://github.com/cwru-robotics/cwru_davinci_calibration_results)

## Usage examples

The following launch files are included with this package:

1. endoscope.launch: launches the stereo endoscope pair:
```bash
roslaunch cwru_davinci_camera endoscope.launch
```
2. endoscope_rect_viewer.launch: launches a viewer of the rectified stereo pair:
```bash
roslaunch cwru_davinci_camera endoscope_rect_viewer.launch
```
3. endoscope_raw_viewer.launch: launches a viewer of the raw stereo pair:
```bash
roslaunch cwru_davinci_camera endoscope_raw_viewer.launch
```
4. endoscope_calibration.launch: launches the calibration functions. The checkerboard information can be defined (default shown):
```bash
roslaunch cwru_davinci_camera endoscope_calibration.launch sq_size:=0.015 sq_dims:=3x5
```
