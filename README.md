# DetectSpeed_and_DataVisualization
 # OpenCV 4.0 Tutorial
[![](https://img.shields.io/badge/opencv-v4.0.0-orange.svg)](https://opencv.org/)       [![](https://img.shields.io/badge/opencv-tutorial-brightgreen.svg)](https://docs.opencv.org/4.0.0/d9/df8/tutorial_root.html)

## Detect Vehicle Speed

### Introduction

This repository contains source code of OpenCV Tutorial application, the environment is python3.0 and opencv4.0.

### Setup and usage
1. If you have previous/other manually installed (= not installed via ``pip``) version of OpenCV installed (e.g. cv2 module in the root of Python's site-packages), remove it before installation to avoid conflicts.
2. Make sure that your `pip` version is up-to-date (19.3 is the minimum supported version): `pip install --upgrade pip`. Check version with `pip -V`. For example Linux distributions ship usually with very old `pip` versions which cause a lot of unexpected problems especially with the `manylinux` format.
3. Select the correct package for your environment:

    There are four different packages (see options 1, 2, 3 and 4 below) and you should **SELECT ONLY ONE OF THEM**. Do not install multiple different packages in the same environment. There is no plugin architecture: all the packages use the same namespace (`cv2`). If you installed multiple different packages in the same environment, uninstall them all with ``pip uninstall`` and reinstall only one package.

    **a.** Packages for standard desktop environments (Windows, macOS, almost any GNU/Linux distribution)

    - Option 1 - Main modules package: ``pip install opencv-python``
    - Option 2 - Full package (contains both main modules and contrib/extra modules): ``pip install opencv-contrib-python`` (check contrib/extra modules listing from [OpenCV documentation](https://docs.opencv.org/master/))

    **b.** Packages for server (headless) environments (such as Docker, cloud environments etc.), no GUI library dependencies

    These packages are smaller than the two other packages above because they do not contain any GUI functionality (not compiled with Qt / other GUI components). This means that the packages avoid a heavy dependency chain to X11 libraries and you will have for example smaller Docker images as a result. You should always use these packages if you do not use `cv2.imshow` et al. or you are using some other package (such as PyQt) than OpenCV to create your GUI.

    - Option 3 - Headless main modules package: ``pip install opencv-python-headless``
    - Option 4 - Headless full package (contains both main modules and contrib/extra modules): ``pip install opencv-contrib-python-headless`` (check contrib/extra modules listing from [OpenCV documentation](https://docs.opencv.org/master/))

4. Import the package:

    ``import cv2``

    All packages contain haarcascade files. ``cv2.data.haarcascades`` can be used as a shortcut to the data folder. For example:

    ``cv2.CascadeClassifier(cv2.data.haarcascades + "haarcascade_frontalface_default.xml")``

5. Read [OpenCV documentation](https://docs.opencv.org/master/)

6. Before opening a new issue, read the FAQ below and have a look at the other issues which are already open.

7. Download the other open source software to support for work
     - Visual Studio Code 1.47.3
     - Python 3.0
     - Cmake 3.18.4
     - Dlib
     - Numpy
     - Matplotlib
     
## Data Visualization
