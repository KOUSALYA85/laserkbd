laserkbd
========

A Low Cost Laser Projection Keyboard designed by RoboPeak

Full Source Code Release

NOTE: all the source code is licensed under LGPL.  No warranty for the sourcecode and the related software.

depend
======
sudo apt-get install libopencv-dev libcurl4-openssl-dev libusb-dev libjsoncpp-dev libkdtree++-dev scons 

build
=====
cd ./laser_kbd_neo

scons

opencv BUG
==========
OpenCV Error: Null pointer (NULL guiReceiver (please create a window)) in cvDestroyWindow, file /tmp/buildd/opencv-2.4.2+dfsg/modules/highgui/src/window_QT.cpp, line 489

apt-get source libopencv-dev

vi modules/highgui/src/window_QT.cpp
line 489, return;
