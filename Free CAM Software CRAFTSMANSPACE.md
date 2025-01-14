# Free CAM Software | CRAFTSMANSPACE
                            Free CAM Software | CRAFTSMANSPACE    [Skip to main content](#main-content) 

 [![](https://www.craftsmanspace.com/sites/default/files/craftsmanspace_logo.svg)](/ "Home") [CRAFTSMANSPACE](/ "Home")

[

Toggle menu

](#)

*   [Free projects](/free-projects)
*   [Free patterns](/free-patterns)
*   [Free 3D models](/free-3d-models)
*   [Free books](/free-books)
*   [Free software](/free-software)
*   [Knowledge](/knowledge)

Type and Press “enter” to Search 

Free CAM Software
=================

This is a list of free and [ open source](#) CAM (computer-aided manufacturing) software packages.

3D modeling for product design

#### \- [FreeCAD - Path workbench](https://www.freecadweb.org/ "FreeCAD software - Path workbench")

#### [\- About FreeCAD](/free-software/about-freecad-free-3d-cad-software.html "About FreeCAD")

The Path workbench is used to produce machine instructions for CNC machines from a [ FreeCAD](#) 3D model. These produce real-world 3D objects on CNC machines such as mills, lathes, lasercutters, or similar. Typically, instructions are a G-Code dialect.

The FreeCAD Path Workbench workflow creates these machine instructions as follows:

*   A 3D model is the base object, typically created using one or more of the Part Design, Part or Draft Workbenches.
    
*   A Job is created in Path Workbench. This contains all the information required to generate the necessary G-Code to process the Job on a CNC mill: there is Stock material, the mill has a certain set of tools and it follows certain commands controlling speed and movements (usually G-Code).
    
*   Tools are selected as required by the Job Operations.
    
*   Milling paths are created using e.g. Contour and Pocket Operations. These Path objects use internal FreeCAD G-Code dialect, independent of the CNC machine.
    
*   Export the job with a g-code, matching to your machine. This step is called post processing; there are different post processors available.
    
    3D printing services
    
    Branding services
    

#### \- [LinuxCNC](http://www.linuxcnc.org/ "LinuxCNC software")

LinuxCNC controls CNC machines. It can drive milling machines, lathes, 3d printers, laser cutters, plasma cutters, robot arms, hexapods, and more.

*       Runs under Linux (optionally with realtime extensions).
    
*       Simple installation on Debian and Ubuntu, or via our Live/Install DVD/USB images.
    
*       Accepts G-code input, drives CNC machines in response.
    
*       Active user community.
    
*       Several different GUIs available.
    
*       Compatible with many popular machine control hardware interfaces.
    
*       Supports rigid tapping, cutter compensation, and many other advanced control features.
    
*       Full source code available under the terms of the GNU GPLv2 (General Public License version 2).
    

#### \- [PyCAM](http://pycam.sourceforge.net/ "PyCAM software")

PyCAM is a toolpath generator for 3-axis CNC machining. It loads 3D models in STL format or 2D contour models from DXF or SVG files. The resulting G-Code can be used with LinuxCNC or any other machine controller.

PyCAM supports a wide range of toolpath strategies for 3D models and 2D contour models. Take a look at the Features page for a full list features.

PyCAM runs on Linux, Windows and MacOS. It is free software licensed under the GPL v3.

#### \- [OpenBuilds software](https://software.openbuilds.com/# "OpenBuilds software")

\- OpenBuilds CONTROL - Machine Interface Controller

OpenBuilds CONTROL is an application for connecting to, and controlling, your CNC, Laser, Plasma or Dragknife machine.

This will allow you to

*   Interface with, and Jog your machine
    
*   Run GCODE Jobs
    
*   Set Zero coordinates
    
*   Integrate with cam.openbuilds.com
    
*   Flatten/Surface your spoilboard / stock
    
*   and even help with your Firmware configuration
    

  
\- OpenBuilds CAM - GCODE Generator

OpenBuilds CAM is a web-based application for converting SVG, DXF and Bitmap drawings, to GCODE for use with your CNC, Laser, Plasma or Dragknife Machine

This will allow you to

*   Import DXF/SVG/PNG/BMP/JPG/Gerber/Excellon files
    
*   Import from a built-in Parts Library
    
*   Setup toolpaths for CNC Routing, Laser cutting, Plasma Cutting and Dragknives
    
*   Generate GCODE
    
*   Send GCODE to OpenBuilds CONTROL
    

#### \- [GRBL](https://github.com/grbl/grbl "GRBL software")

Grbl is a no-compromise, high performance, low cost alternative to parallel-port-based motion control for CNC milling. It will run on a vanilla Arduino (Duemillanove/Uno) as long as it sports an Atmega 328.

The controller is written in highly optimized C utilizing every clever feature of the AVR-chips to achieve precise timing and asynchronous operation. It is able to maintain up to 30kHz of stable, jitter free control pulses.

It accepts standards-compliant g-code and has been tested with the output of several CAM tools with no problems. Arcs, circles and helical motion are fully supported, as well as, all other primary g-code commands. Macro functions, variables, and most canned cycles are not supported, but we think GUIs can do a much better job at translating them into straight g-code anyhow.

Grbl includes full acceleration management with look ahead. That means the controller will look up to 18 motions into the future and plan its velocities ahead to deliver smooth acceleration and jerk-free cornering.

    Licensing: Grbl is [ free software](#), released under the GPLv3 license.

#### \- [CAMotics](https://camotics.org/ "CAMotics software")

With CAMotics, you can simulate 3-axis GCode programs for CNCs and visualize the results in 3D. CAMotics runs on Linux, OS-X or Windows. It's fast, easy to use and best of all [ Open-Source](#) and free.

With the power to simulate your CNC tool paths you will avoid dangerous and expensive mistakes. By looking at the built-in examples and using the online documentation you'll be running your own simulations in no time. And, if you need more help, we'll be happy to answer your questions via the discussion group.

CAMotics aims to be a useful CNC simulation platform for the DIY and Open-Source community. CAMotics should serve the highly technical user but remain simple and user friendly enough to support less techie types as well.

Features:

1.  Fast 3-axis cut-workpiece simulation with 3D visualization.
    
2.  Simulates cylindrical, conical, ballnose, spheroid and snubnose tool shapes.
    
3.  Tool path 3D visualization.
    
4.  Multi-threaded rendering can take advantage of multi-processor CPUs.
    
5.  GCode parsing, simulation, verification and annotation.
    
6.  In application GCode and TPL view and edit.
    
7.  Supports LinuxCNC (AKA EMC2) O-codes.
    
8.  Export cut workpiece to STL file.
    
9.  Tool table editing.
    
10.  Add height probing to 2D GCode files. Very useful for circuit board cutting and metal engraving.
    
11.  2D GCode path optimization. (in progress #11)
    
12.  Operates in Windows and Linux.
    
13.  Released under the GPL v2+ license.
    

#### \- [Blender CAM](http://blendercam.blogspot.com/ "Blender CAM software")

Blender CAM is an open source solution for artistic CAM - Computer aided machining - a g-code generation tool. Blender CAM is an extension for the free open-source Blender 3d package.  It has been used for many milling projects, and is actively developed. If you are a developer who would like to help, don't hesistate to contact me.

This extension is free of charge, however you can donate to support the development and appreciate the work which has allready been done. There is currently no warranty for the results from blender CAM - you have to check your paths before use. Blender CAM has been tested with success in my studio. I wouldn't recommend Blender CAM for metalworking now, be carefull if you try it. 

Features:

*       Several milling strategies for 2D and 3D
    
*       Cutter types: ball, flat, v-carve with various angles
    
*       work with 3d data or depth images
    
*       Layers and skin for roughing.
    
*       Inverse milling 
    
*       Various options for ambient around model
    
*       protection of vertical surfaces
    
*       stay low - option for movement
    
*       material size setup
    
*       simulation of 3d operations
    
*       Background computing of the operations, so you can continue working
    
*       helix entry, arc retract, ramp down for some of the strategies.
    
*       Automatic bridges for cutout operation
    
*       Chain export and simulation
    

#### [\- DXF2GCODE](https://sourceforge.net/projects/dxf2gcode/ "DXF2gcode")

DXF2GCODE is a tool for converting 2D (dxf, pdf, ps) drawings to CNC machine compatible GCode. Windows, Linux, and Mac support by using python scripting language.

Features:

*       Integration in EMC2
    
*       Fully adjustable Postprocessor
    
*       G0 moves reduction by route optimization
    
*       Import of DXF, PDF and PS files
    
*       Improved accuracy for splines import by Line and Arc's
    
*       Mill parameter specification by layers
    
*       Drag knife and lathe support
    
*       Breaks a.k.a Tabs support
    
*       AutoCAD Blocks and Inserts
    
*       Multiple tools
    
*       Multiple language support: English; German; French; Russian
    
*       3D viewer
    

[![](https://www.craftsmanspace.com/sites/default/files/inline-images/free_software_alternatives.webp)
](https://www.craftsmanspace.com/free-software/free-alternatives-to-commercial-software.html "Free alternatives to commercial software")

#### [![](https://www.craftsmanspace.com/sites/default/files/x_logo.svg)
](https://x.com/Craftsmanspace "Craftsmanspace X page")    [![](https://www.craftsmanspace.com/sites/default/files/pinterest.png)
](https://www.pinterest.com/Craftsmanspace/ "Craftsmanspace Pinterest page")

[![](https://www.craftsmanspace.com/sites/default/files/inline-images/freecad_tutorials.webp)
](https://www.craftsmanspace.com/freecad-tutorials "Craftsmanspace FreeCAD tutorials")

[Free CAD/CAM/CAE/PDM software](/free-software/cad-cam-cae-pdm-software.html)
-----------------------------------------------------------------------------

*   [Free 2D CAD software](/free-software/free-2d-cad-software.html)
*   [Free 2D and 3D CAD viewers](/free-software/free-2d-and-3d-cad-viewers.html)
*   [Free 3D CAD software](/free-software/free-3d-cad-software.html)
*   [Free 3D modeling software](/free-software/free-3d-modeling-software.html)
*   [Free 3D printing software](/free-software/free-3d-printing-software.html)
*   [Free CAE software](/free-software/free-cae-software.html)
*   [Free CAM Software](/free-software/free-cam-software.html)

Showroom gallery
----------------

[![](https://www.craftsmanspace.com/sites/default/files/inline-images/craftsmanspace_showroom_gallery.jpg)
](/craftsmanspace-showroom "Showroom gallery")

**Copyright©2025 Craftsmanspace.**  All Rights Reserved.              

[Disclaimer](/disclaimer)      |      [License Agreement](/license-agreement)      |      [Showroom gallery](/craftsmanspace-showroom "Craftsmanspace showroom gallery")      |      [Contact Us](/contact-us)   

sfy39587stp18