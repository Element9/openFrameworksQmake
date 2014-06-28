openFrameworksQmake
===================

This repository contains a .pri file which can be used to easily create openFramworks projects in Qt Creator on Windows. Just define OPEN_FRAMEWORKS and include this .pri file into your .pro file.

For example:

    OPEN_FRAMEWORKS = D:/Dev/Libs/openFrameworks/0.8.1
    include(D:/Dev/Projects/OFTest01/openFrameworks.pri)
	
.pri file contains INSTALLS target, so you can add a make step in to your project with "install" argument to have openFrameworks dll files copied to the build output folder.
	
Tested with 0.8.1 version of openFrameworks, qmake from Qt 5.2, Qt Creator 3.1. Tested only with shadow build.