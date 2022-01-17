X-Carve CNC Router
======================

Installing Easel Post Processor
-------------------------------

This tutorial will walk you through the process of installing the Easel Post Processor. This post processor is required to use the X-Carve CNC Router. 

1)	Launch Easel, navigate to File -> Import G-Code 

.. figure:: ../_static/images/X1.PNG
    :figwidth: 450px
    :target: ../_static/images/X1.PNG

2)	The menu below will appear. Before you import your part, you’ll need to download and install the post processor. Select Autodesk 360 and choose your device (i.e. Mac or PC) 

.. figure:: ../_static/images/X2.PNG
    :figwidth: 450px
    :target: ../_static/images/X2.PNG

3)	Next launch Autodesk 360. Go to the Fusion 360 Account Ribbon on the top right corner of your screen and select preferences
 
.. figure:: ../_static/images/X3.PNG
    :figwidth: 450px
    :target: ../_static/images/X3.PNG

4)	Go to the left-hand bar and select Manufacture, then select the check box “enable cloud libraries”. Press Apply, then OK. 
 
.. figure:: ../_static/images/X4.PNG
    :figwidth: 450px
    :target: ../_static/images/X4.PNG

5)	Next you need to navigate tot eh fusion 360 online portal. Go to File, then select “View Details on Web” 
 
.. figure:: ../_static/images/X5.PNG
    :figwidth: 450px
    :target: ../_static/images/X5.PNG

6)	This will bring you to the part page, click the “home” button to navigate to the main menu. 
 
 .. figure:: ../_static/images/X6.PNG
    :figwidth: 450px
    :target: ../_static/images/X6.PNG

7)	Navigate to the menu named “assets” 

.. figure:: ../_static/images/X7.PNG
    :figwidth: 450px
    :target: ../_static/images/X7.PNG

8)	The CAMPosts folder holds the post processors for Fusion 360. Upload the Easel Port Processor file we downloaded earlier to this folder.  

 .. figure:: ../_static/images/X8.PNG
    :figwidth: 450px
    :target: ../_static/images/X8.PNG
 
9)	Now the Easel post processor will be available for you to use in Fusion 360
This tutorial was generated using the following video: 
https://youtu.be/DFwXdnKzg2I


Changing the Router Bit
-------------------------------

CRITICAL! UPLUG THE ROUTER. 
Safety Reminder: Router bits are very sharp, only handle the bits with cut proof gloves. 
To remove the bit from the router you will need to press the small yellow button on bottom right hand side of the router (just above the router). While depressed, this button locks the rotation of the router. 

 .. figure:: ../_static/images/X9.PNG
    :figwidth: 450px
    :target: ../_static/images/X9.PNG

Using the spanner wrench shown in the photo below (while holding the button in) loosen the router mount by turning the spanner counter clockwise (CCW).

 .. figure:: ../_static/images/X10.PNG
    :figwidth: 450px
    :target: ../_static/images/X10.PNG

 .. figure:: ../_static/images/X11.PNG
    :figwidth: 450px
    :target: ../_static/images/X11.PNG

The router mount does not need to be removed fully, unless you’re using a bit with a larger shank. In which case the collet would also need to be replaced (inside the router mount). It’s been removed in the photo below to show the collet. The collet is used to hold the bit in place and can be replaced to use bigger (or smaller) bits. The bit can travel freely in the collet until the router mount is tightened. 

 .. figure:: ../_static/images/X12.PNG
    :figwidth: 450px
    :target: ../_static/images/X12.PNG

Slide the old bit out of the collet and slide the new bit into the collet. To ensure you’re using the intended bit you can check the color (per the bit guide link) or check the top of the color for the bit description. 

 .. figure:: ../_static/images/X13.PNG
    :figwidth: 450px
    :target: ../_static/images/X13.PNG

 .. figure:: ../_static/images/X14.PNG
    :figwidth: 450px
    :target: ../_static/images/X14.PNG

The bit should slide freely in the collet. Slide the router mount back onto the router router and twist it into place. The bit should move freely in the collet until the clearance between the router mount and the router is approximately 0.3”. 

 .. figure:: ../_static/images/X15.PNG
    :figwidth: 450px
    :target: ../_static/images/X15.PNG

After this point you can still twist the router mount but you’ll notice increasing friction on the shank of the router bit. Move the bit up into the collar until the spacer stops it from moving further, and then hand tighten it until its snug. The bit will no longer slide easily up and down in the router mount. 

 .. figure:: ../_static/images/X16.PNG
    :figwidth: 450px
    :target: ../_static/images/X16.PNG

Next use the spanner to tighten the router mount in place. Similar to when you were removing the mount, hold the yellow button to stop the router from rotating. 

 .. figure:: ../_static/images/X17.PNG
    :figwidth: 450px
    :target: ../_static/images/X17.PNG

That’s it! You’ve changed the bit! 


Machine Set-Up
-------------------------------

Setting up the X-Carve
The fist step to using the X-Carve will be installing the Easel Driver on your computer. You’ll be prompted to download the driver when you press Carve:

 .. figure:: ../_static/images/X18.PNG
    :figwidth: 450px
    :target: ../_static/images/X18.PNG

 .. figure:: ../_static/images/X19.PNG
    :figwidth: 450px
    :target: ../_static/images/X19.PNG
  
After the driver is installed, you can plug the USB connection from the X-Carve DC P/S Interface into your computer. Power on the Interface (make sure the toggle is in the ON position before you do).

 .. figure:: ../_static/images/X20.PNG
    :figwidth: 450px
    :target: ../_static/images/X20.PNG

Press the Carve button in Easel. If the machine does not connect automatically you’ll need to identify which COM port your USB is connected to. Open the Device Manager on your PC.

 .. figure:: ../_static/images/X21.PNG
    :figwidth: 450px
    :target: ../_static/images/X21.PNG

Look for the section labelled Ports (COM & LPT). A connected device will be clear to read, while unused ports will be opaque. In this case we’re connected to COM port 4. Enter 4 on the Easel connection screen to connect to X-Carve. 
Now you’ll have control of the machine! 
By clicking the Green Arrow button at the top of the screen you’ll be able to jog the router. Now you can move the router around the bed by using the arrow keys (you’ll need to toggle that on as shown in the screenshot below. 

 .. figure:: ../_static/images/X22.PNG
    :figwidth: 450px
    :target: ../_static/images/X22.PNG

Try jogging the router around the bed!
Next press the Carve Button. You will be prompted to set up the machine. 

 .. figure:: ../_static/images/X23.PNG
    :figwidth: 450px
    :target: ../_static/images/X23.PNG

Press set up your machine, this X-Carve was purchased in 2017, so select the appropriate set up: 

 .. figure:: ../_static/images/X24.PNG
    :figwidth: 450px
    :target: ../_static/images/X24.PNG

Enter the following settings:

X-Carve
X-Controller
1000mm x 10000mm
ACME Threaded Rod 
DeWalt 611
Dust Shoe = Yes 

 Next you’ll need to confirm the machine is wired correctly by jogging it. Press the indicators and confirm that the machine moves correctly in the X – Y – Z directions. 
 
 .. figure:: ../_static/images/X25.PNG
    :figwidth: 450px
    :target: ../_static/images/X25.PNG

The router on this machine has been set up manually (this means it must be adjusted at the top of the router). You will set up the router to confirm manual operation. There is a speed chart for corresponding numerical values to RPM in the X-Carve Bit Guide. 

 .. figure:: ../_static/images/X26.PNG
    :figwidth: 450px
    :target: ../_static/images/X26.PNG

This machine does not have homing switches. 
 
This machine does have a Z-Probe
 
Now you’re done the basic set-up! You can now start carving!


Test Cut
-------------------------------
For our test cut we’re going to be using 1/8” particle board. The X-Carve default is shown below: 

 .. figure:: ../_static/images/X27.PNG
    :figwidth: 450px
    :target: ../_static/images/X27.PNG

Some important things to note: 
You need to adjust the size of your stock (length / width / thickness)
You need to secure your stock 
You need to determine your zero position 
You need to adjust the depth of each profile cut 

First you need to measure your stock.
Grab the measuring tape from the toolbox and do a check of your material size: 
 
 .. figure:: ../_static/images/X28.PNG
    :figwidth: 450px
    :target: ../_static/images/X28.PNG
 
 .. figure:: ../_static/images/X29.PNG
    :figwidth: 450px
    :target: ../_static/images/X29.PNG

The effective stock size we have for this cut is 31” x 16” (at 1/8” thick)

Next we need to secure the stock. 

You can secure the stock to the bed by using the provided wooden clamps. There is a grid pattern throughout the table with threaded inserts to all the clamps to be mounted. Secure the part from all four sides using a M5 hex key. If it not possible to secure the material from all four sides then an alternative clamping method must be used. 
Make sure that the clamps stop the stock from moving, and they are applying downward force on the stock. If you’re not sure if your stock is secure, try pushing it firmly from all four sides in various places. If the material can shift then you need to secure the material differently. 
You’ll notice another issue with the way the example above is secured. The bottom left and right corners aren’t secured. Given this is a thin piece of material, there is a chance for the material to rise as the router is cutting. This will cause the machine to lose position, spoiling your material and leaving a poor cutting finish. For thin materials, it’s best to screw them directly to the spoil board, or use double sided tape. 
For a better overview of securing a part to the router bed, see the “Setting Up the Evo-One Tutorial”. 

Next we need to identify the zero position. 

This will be done as part of your “Carve” operation. First position your part on the stock. Easel will preview the cut on the right side of the screen. Ensure your cut fits inside the material. 

 .. figure:: ../_static/images/X30.PNG
    :figwidth: 450px
    :target: ../_static/images/X30.PNG

Press Carve. Easel will ask you to confirm your material thickness. Measure the thickness with a set of calipers to ensure you’ve entered the right value. 

 .. figure:: ../_static/images/X31.PNG
    :figwidth: 450px
    :target: ../_static/images/X31.PNG
 
Next confirm the part is secured. As mentioned above, try your best to move the stock. If it can shift “AT ALL” then the part needs to be secured again. 
Then easel will ask you to confirm the bit to be used. For this cutting operation we’re going to use the 2 Flute UpCut Bit. For details on bits see the X-Carve Bit Guide (link). 

 .. figure:: ../_static/images/X32.PNG
    :figwidth: 450px
    :target: ../_static/images/X32.PNG 

If you need to change the bit, go back to “Changing the Router Bit”.

Next you’ll need to zero your machine. Here are some best practices for zeroing the machine: 
Try to position the bit as close to the bottom left corner of the stock as possible
Leave enough clearance on the X and Y axis to ensure that the router will not collide with the clamps. Best practice is to measure how far onto the part the clamps are to avoid hitting them. 

 .. figure:: ../_static/images/X33.PNG
    :figwidth: 450px
    :target: ../_static/images/X33.PNG 

Use a piece of paper when determining your Z zero. Slowly lower the resolution of the movement until the paper doesn’t move between steps. Alternatively, use the included Z-Probe.

 .. figure:: ../_static/images/X34.PNG
    :figwidth: 450px
    :target: ../_static/images/X34.PNG 

Now you’re ready to start carving!


Bit and Router Parameters
-------------------------------

Before 

.. figure:: ../_static/images/X.PNG
    :figwidth: 450px
    :target: ../_static/images/X.PNG


Using Easel for Simple Cuts
-------------------------------

Before 

.. figure:: ../_static/images/X.PNG
    :figwidth: 450px
    :target: ../_static/images/X.PNG

Importing G-Code to Easel
---------------------------------

Before 

.. figure:: ../_static/images/X.PNG
    :figwidth: 450px
    :target: ../_static/images/X.PNG