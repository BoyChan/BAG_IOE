# BAG_IOE

*Note: This file is best viewed with support for the Markdown markup language.*

## The program, in brief

The method is writen by C++/Qt and osgEarth in Microsoft Visual Studio 2015(x64). These are the highlights:

1. The BIM model (.ifc) need to be converted into the supported format(.osgb) in the osgEarth. The converted tool can easily be found in [IfcPlusPlus](https://github.com/ifcquery/ifcplusplus)
2. Experimental data (orginal IFC file and custom format) can be found in "/data".
3. The custom format is a directory. Beisdes, the directory name includes the bounding sphere and its name. For example, "32.2058,1.46398,-3,59.8065,BUILDING.bim" represents that the bounding sphere ( center(32.2058,1.46398,-3) and radius=59.8065) and name "BUILDING".

## Quick Start

### Windows

The program can be organized by VS 2015(x64), if you can meet the following requirements, you can choose to download "" including complete dependent files and the solution can be directly compiled and run.
* Windows 10 x64
* Microsoft Visual Studio 2015(x64) and Qt VS addin
* Qt 5.8 x64

## Building instruction

For VS IDE proceed as follows:

1. Install Qt 5.8 (Desktop OpenGL version)
2. Download [OpenSceneGraph 3.4.0](http://www.openscenegraph.org/) and [osgEarth 2.8](https://github.com/gwaldron/osgearth) , run CMake to build it and set the paths to Qt.
3. Install Qt VS addin, configure it to use the same Qt files like the environment variable QTDIR. 
4. Open "MainWindow.sln" and set dependent environments.
5. First compile "BIM" and then compile "MainWindow".

## Linux

Qt 5.8, OpenSceneGraph 3.4 and osgEarth 2.8 both are supported in Linux, so the program may be compiled.

![Demo1](https://github.com/BoyChan/BAG_IOE/blob/main/Demo1.png)

![Demo2](https://github.com/BoyChan/BAG_IOE/blob/main/Demo2.png)

