ofxLaser
=========

An openFrameworks addon for controlling one or more iLDA laser projectors, it's particularly good at rendering graphics. It currently works with the Etherdream controller, but more DACs to be added in the future.

Safety Notice
=============
**LASERS ARE DANGEROUS - USE THIS SOFTWARE AT YOUR OWN RISK**. Always have an emergency stop button at hand and do not let anyone enter the laser exposure area. Take laser safety training and get licenced to use high power lasers in your locale. In the UK I can recommend [this one](https://www.lvroptical.com/display.html)

Features
----------
* Can draw any vector shape to the laser with a simple function calls
* Shapes are sorted to find the optimal path for the laser
* Can control multiple lasers (limited only by CPU and network speed)
* Many calibration options for blanking - colour change offset, pre/post blanks, pre/post on points
* Specify laser speed and acceleration for each shape using "render profiles" 
* Output warping to compensate for perspective distortion
* Multiple zones can be sent to multiple projectors and individually warped for mapping onto separate planes
* Colour calibration system to compensate for laser power to brightness curves
* Full rewrite of the Etherdream library using Poco sockets, very reliable
* Shapes take into account the current transformation matrix, so should work with ofTransform, ofRotate, and ofScale
* Should work with 3D coordinates but needs further testing
* Cross platform - mostly tested on OSX, but should work on Windows and Linux

Roadmap
-----------
* Automatic discovery of Etherdreams (currently requires the DAC IP address)
* Masking of individual areas with varying levels
* Optimisation of point generation and sending to DACs
* IDN Ilda Digital Network support

Licence
-------
The code in this repository is available under the [MIT License](https://secure.wikimedia.org/wikipedia/en/wiki/Mit_license).  
Copyright (c) 20012-2018 Seb Lee-Delisle [seb.ly](http://seb.ly)

Installation
------------
Copy to your openFrameworks/addons folder.


Dependencies
------------
ofxXmlSettings (comes with oF)
ofxGui (comes with oF)
ofxOpenCv (comes with oF)
ofxPoco (comes with oF)

Compatibility
------------
openFrameworks 0.10 - currently tested with 0.10


Known issues
------------

Version history
------------

