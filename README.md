# `vision_utils_tests`

[![Build Status](https://travis-ci.org/UC3MSocialRobots/vision_utils_tests.svg)](https://travis-ci.org/UC3MSocialRobots/vision_utils_tests)

`vision_utils_tests` is a [ROS](http://www.ros.org/) package
to test the package `vision_utils`.

How to install
==============

Dependencies from sources
-------------------------

Dependencies handling is based on the [wstool](http://wiki.ros.org/wstool) tool.
Run the following instructions:

```bash
$ sudo apt-get install python-wstool
$ roscd ; cd src
$ wstool init
$ wstool merge `rospack find vision_utils_tests`/dependencies.rosinstall
$ wstool update
```

Dependencies included in the Ubuntu packages
--------------------------------------------

Please run the ```rosdep``` utility:

```bash
$ sudo apt-get install python-rosdep
$ sudo rosdep init
$ rosdep install vision_utils_tests --ignore-src
```

Build package with Catkin
-------------------------

```bash
$ catkin_make --only-pkg-with-deps vision_utils_tests
```
