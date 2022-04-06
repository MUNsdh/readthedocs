Profilometer
============
(picture of profilometer)
.. image:: ../_static/images/Profilometer_0.png
   :width: 1000px

The Student Design Hub lab has a device called a "profilometer". It develops a 3D image by running a laser across an object and recording the height of the laser beam at each increment. The profilometer uses a Trispector 1060 sensor to record data and an Arduino Uno to control the motor on the apparatus. These are both connected to a router, allowing any computer that is connected to that router to communicate with the sensor and the Arduino wirelessly. A program was created to make it easier for a computer to control the motor on the apparatus without having to be plugged into the Arduino. The steps for downloading and using this program are detailed below. The software required to communicate with the sensor is called SOPAS Engineering Tool, which can be installed from `here. <https://www.sick.com/ca/en/sopas-engineering-tool/p/p367244>`_

Installing and Using the Program for Controlling the Motor
----------------------------------------------------------
The ZIP file containing the program executable for controlling the profilometer can be downloaded from this link: 

:download:`Download ZIP File <Profilometer Controller.zip>`.

After downloading and extracting the ZIP file, open the folders until you see this:
(Picture of directory containing program executable)
.. image:: ../_static/images/Profilometer_1.png
   :width: 1000px
   
This is file contains an executable file called "Profilometer.exe". This is the program. **Do not move the executable outside of this folder**. If you wish to make this file quickly accessible, you will have to create a shortcut for it.

The Scanning Process
--------------------
The first step to producing a scan is to place an object under the scanner. To ensure the most detailed scan possible, place the item such that there is minimal overhang. The sensor can only see features of the object from above, so overhangs will not be included in the profile.
(diagram of overhang vs. no overhang)
.. image:: ../_static/images/Profilometer_2.png
   :width: 1000px
   
It is recommended that you place the object ~1 ft ahead of the laser line so that you have time to trigger the sensor.
