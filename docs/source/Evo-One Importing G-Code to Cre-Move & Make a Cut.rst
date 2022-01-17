Evo-One Importing G-Code to Cre-Move & Making a Cut
===================================================

picture 1

1. Turn on the Computer

2. Plug in the E-Stop and Z-Probe

picture 2,3

3. Connect the PC by USB, wait for Drivers to Install 
	a. If drivers do not install automatically visit: https://makerdreams.it/download-software/
	
4. Power on the machine by pressing the power switch 

picture 4

5. Launch Cre-Move
	a. You can download Cre-Move from the Makerdreams site: https://makerdreams.it/download-software/
	b. NOTE: unzip the folder and save it somewhere on your computer. The EXE file must be run from the folder with the reference files or it will not move
	c. NOTE: Download CRE-MOVE PRO 2021
	d. NOTE: Cre-Move’s UI doesn’t stretch with resolution. It works best on a 1080p screen (for laptops) or on a computer monitor.
	
6. In Cre-Move under “Connection” connect to the machine

picture 5

7.  Navigate to the Control menu, the machine will show an Alarm. Press Reset. Then unlock the machine. 

picture 6

8. Next hit the home button to teach the machine where the machine zero is. This will teach the machine where X:0, Y:0, Z:0 from a machine reference should be

picture 7

9. Next jog the machine so the spindle is directly over the stock. You can jog the spindle by using the directional buttons on screen. There are two movement options: 
	a. Continuous: The spindle will move while the button is pressed
	b. Step: The spindle will move by the specified step number
	
Continuous is great for getting the machine in the general position quickly. Then you can use step to precisely move the spindle. Move the machine at 1 step for higher accuracy, and 10 steps for quicker repositioning. 
picture 8, 9

10. Zero the machine in the z-direction by placing the probe directly under the bit. Then press Z-Probe. The machine will touch the probe and then move back to the top of its reference geometry. Now the machine knows the z-position of the stocks surface. 

picture 10

picture 11

11. Next zero the x-y axis by moving the machine to the bottom left corner of the stock. This should be the x-y position of the origin in your gcode. Look back at your toolpaths to determine where you set the stocks origin to be. In this case it’s the bottom left corner of the stocks top surface. Try to align the center of the bit with the corner of the stock.

picture 12
picture 14

12. Now you can import your GCode. Go to the G-Code tab and press Open. Navigate to your G-Code exported from fusion 360 and select it. The g-code will preview in the screen to the left. 

picture 15

picture 16

Of the preview looks correct, press Play and watch the machine do the rest! 

picture 17

NOTE: if the machine is behaving in a way that doesn’t look correct, or it is going to damage something press the E-STOP! 

picture 18

Smile! You made your first cut on the MakerDreams Evo-One!

picture 19

