# glskybox

A simple python tool for converting skysphere texture to skybox.

## Requirements

* [PyOpenGL](http://pyopengl.sourceforge.net/) The Python OpenGL Binding
* [Pillow](https://pypi.python.org/pypi/Pillow) Python Imaging Library

`pip install -r requirements.pip`

## Usage

    usage: glskybox.py [-h] [-o OUTPUT] [-s SIZE] [-f] FILE [FILE ...]
    
    Convert skydome texture to skybox
    
    positional arguments:
      FILE                  source file name
    
    optional arguments:
      -h, --help            show this help message and exit
      -o OUTPUT, --output OUTPUT
                            destination path
      -s SIZE, --size SIZE  output image size
      -f, --overwrite       overwrite existing output
      
    for python 3.5 win64, add a whl install file
        pip install PyOpenGL-3.1.1-cp35-cp35m-win_amd64.whl
Example:

Use a photo taken by [PhotoSphere](https://www.google.com/maps/streetview/publish/) app, then run:

`python glskybox.py your_sphere_photo.jpg`

Check out the result in output/ directory.

If you give a directory as input, it will traverse all files inside it and render them.
