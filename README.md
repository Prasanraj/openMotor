openMotor
==========

Overview
--------
openMotor is an open-source internal ballistics simulator for rocket motor experimenters. The software produces estimates of a rocket motor's chamber pressure and thrust based on input such as propellant properties and grain geometry. It uses the Fast Marching Method to determine how a propellant grain regresses, which allows the use of arbitrary core geometries. 

Current Features:
* Metric and imperial units
* Support for common grain geometries such as BATES, Finocyl, Star and more
* A propellant editor that allows the user to enter the properties of as many propellants as they wish
* The grain editor displays how a grain will regress to cut down on the guesswork involved in tweaking geometry
* ENG file exporting
* A UI that supports saving and loading designs along with undo and redo.

Planned Features:
* Erosivity simulation
* Loading custom grain geometry from SVG files
* Burnsim importing and exporting
* Detailed output of every calculated parameter at any time and position along the motor

The calculations involved were sourced from Rocket Propulsion Elements by George Sutton and from Richard Nakka's website (https://www.nakka-rocketry.net/rtheory.html).

Usage
-------
The easiest way to use openMotor is to navigate to the 'releases' tab above and download latest version for your system. From there, just unzip the file and run it. 

Alternatively, you can run it from source. To do so, clone the repository, navigate to the directory, and run main.py. The program is currently being developed using python 3.6, but it also works with 3.7. Its dependencies include PyQt5, matplotlib, numpy, scipy, scikit-fmm, and scikit-image.

License
-------
openMotor is released under the GNU GPL v3 license. The source code is distributed so you don't have to trust the calculations are being done correctly and can check for yourself if you doubt the results.

Contributing
------------
As openMotor is open source, one of the goals of the project is to have as many eyes on the code as possible. I believe this is the best way to avoid bugs and also the easiest way to get new features added to the software. If you have ideas on how to improve the program or find an error, please open an issue ticket for discussion or file a pull request if you would do it yourself.
