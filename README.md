# OD
---

This project is used to compute the distance from a known object in an image to our camera.

To accomplish this task we utilized the triangle similarity, which requires us to know two important parameters prior to applying our algorithm:
 - 1) The width (or height) in some distance measure, such as inches or
    meters, of the object we are using as a marker.
 - 2) The distance (in inches or meters) of the camera to the marker in
    step 1.
 - 3) Computer vision and image processing algorithms can then be used to
    automatically determine the perceived width/height of the object in
    pixels and complete the triangle similarity and give us our focal
    length.
 - 4) Then, in subsequent images we simply need to find our marker/object
   and utilize the computed focal length to determine the distance to
   the object from the camera.

## Dependent Packages
* [numpy](https://pypi.python.org/pypi/numpy)
* [OpenCV-Python](http://docs.opencv.org/master/dd/dd5/tutorial_py_setup_in_fedora.html)

## Usage
* initialize the list of images in line 32.
* python computeDistance.py
