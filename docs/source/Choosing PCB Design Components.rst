Choosing PCB Design Components
==============================
**The answer is always in the datasheet.**

PCB Components
--------------
Components are the electrical devices that form electrical circuits. Common components such as resistors, capacitors, 
and inductors are either through hole components (THT) or surface mount devices (SMD). All this refers to is how they 
are mounted on the circuit board. THT components require a hole in the board where the component’s leads are soldered as
seen below. While SMD components are placed directly on the surface of the boards seen below.


THT Capacitor being mounted on a board

SMD integrated circuit being mounted on a circuit board

Electronic components, such as resistors and switches, can be purchased from distributors such as Digikey, Mouser, and Newark that have a wide variety of stock and well organized inventories with accurate component datasheets - component datasheets are very important. 

Component datasheets are manuals that explain what a component can do, how to use it, and contain every technical information related to the part. It contains the component’s dimensions, maximum input and output values, and sample circuits that can be built with it. Learn more here.

Digikey
-------

Digikey has the most variety of all distributors. As such, the inductor in figure XX from digikey will be used as an example: 
The bolded part number at the top is the manufacturer's product number i.e. the component is always known by this part number on all supplier sites. While the Digikey part number is local for within the Digikey database only.
The description and the detailed description sections highlight the most important attributes for selecting a component. It varies from component to component.

With understanding electrical components, the more you work with and read about them, the better you will understand them. An easy google search about a section you do not understand will provide you with a brief overview and a starting point to understanding the component. You can then look into the datasheet for a more technical perspective.

Searching Digikey’s Inventory
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
On your first visit to the digikey site, you arrive at a homepage where you can search their inventory. As seen below, the component name can either be searched or selected.


Searching for a capacitor yields the below information. Ceramic capacitors are the most common with over 600,000 items so we select that.


It is not easy to go over 656,480 capacitors. Thus, we filter the selections using the important properties in the product description learnt in the previous section: 1.22 - Digikey.


Components Selection
--------------------
F1TENTH Powerboard

The power distribution board of the car is divided into three sections; the buck-boost converter, the boost converter, and the peripherals. The objective of the power distribution board is as the name implies, to distribute the battery power to other components of the car’s system. These other components are the autonomy elements like the VESC, Jetson computer, and the Lidar.

The thought process of designing this powerboard simply involved asking the question

 **“how do I distribute the power of a 11.1V 3S battery to a Jetson and a Lidar ?”**

 Note that the battery was chosen as the power source because a car is mobile and needs to move. It cannot be connected to a power socket on a wall. The answer to this question involves looking for the power requirements of these autonomy elements from their respective datasheets:

**Jetson NX:** has a maximum continuous current draw of 4.4A with a supply voltage between DC 10 - 30V 
Hokuyo UST-20LX Lidar: has a maximum current draw of 450 mA  with supply voltage DC 9 - 20V

Now that we know the conditions under which these autonomy elements will function, we create these conditions. Keep in mind that both the Jetson and lidar take a voltage supply within the range of DC 10 - 20V but the optimal voltage is decided to be 12V as it is a common DC voltage.

**Buck-boost converter**
Jetson NX and Hokuyo UST-20LX Lidar: The Jetsn and Lidar both need 12V  to function but the battery outputs 11.1V. We will need to step up the 11.1V output from the battery to a 12V output using a switching regulator i.e. a buck-boost converter. It is important to note that voltage can either be stepped up using a converter or transformer but the fundamental difference between the two is a transformer only works for AC voltage, while a converter works for DC voltage - which is being used. 

**Buck converter**
This converter is arbitrary and designed as part of the board for flexibility. It steps down the 11.1V battery to a 5V output in the case of connecting components with an operating voltage of 5V.

**Peripherals**
The peripherals section entails components that will interface all external hardware with the board (both the autonomy elements and the battery), components that optimize the board’s flexibility, and components that optimize the functionality of the board. See below the functions of these peripherals;

The Jetson NX can be plugged into a 12V output terminal block and the Hokuyo UST-20LX Lidar can be plugged into a 12V output terminal block or a XT30 connector with a 12V output. 

Other elements in this section like the 5V terminal block and the 8 position connector labeled as ‘Hokuyo 10LX’ were all designed as part of the board to optimize design flexibility.

Other elements like the switches, LED, and barrel jack all optimize the functionality of the board. The LED will indicate when the board is powered on. The barrel jack will be used as the bench power source for testing the powerboard. With the two switches, one will power on and off the board and the other will be used to switch between either of the two power sources; the battery or the barrel jack.

The battery and balancer connectors connect the battery (the power source) to the board.

How to Select the Components on Digikey
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Based on the power requirements of the autonomy elements like the Jetson i.e. operating voltage and maximum current, we choose the components for the board with respect to these requirements. Let’s choose components from the first section of the circuit to the last section:

**Buck boost converter:** select max voltage output as 12V and max current output as 5A based on the power requirements of the Jetson and Lidar previously established. You will notice that there are a ton of options to choose from, filter through all the selections and view their datasheets to finalize the decision. When looking at the datasheet, focus on the applications circuit section, description, and part features.

There is a ‘typical application circuit’ section that displays sample applications of this component. Ideally, you should find the circuit for your specific application like the one below to boost the output voltage. The subcomponents of the system like the capacitors, inductors, and resistors are simply components rated at either a power rating calculated using the power formula V^2/R for resistors, the voltage rating for capacitors, and the current rating for  inductors. 5A and 5V are the maximum operating current and voltage. All the resistors used are rated at 0.25W, the inductors are rated above 5A, and the capacitors are rated above 12V.


Application of a buck boost converter

**Buck converter:** similar to the buck boost, the power requirements are maximum 5V output voltage and 5A output current. The datasheet entails the circuit below which can be exactly copied and modified using the table from the datasheet to perform the function of stepping down the voltage to 5V.




**Peripherals:** the most important thing to remember is that current is drawn. The current rating of the peripheral components is dependent on the load it connects to. It is important to make a mental note of the function of each connector before selecting the component.

* 5V and 12V terminal blocks - can connect the lidar or jetson with the jetson having a max continuous current draw of 4.4A. The terminal blocks should be rated at above 4.4A.
* 8 position connector - can connect the lidar with a max current draw of 450 mA. It should be rated at above 450mA.
* Balancer and battery connector -  The balancer and battery connectors require that the connectors of the battery and balancer are a match for them. The type of connector on the battery is used to determine the connector for the board. 
* Switches, LED, barrel jack -  These should be rated above 5A and 12V since they are not connected to loads but the max current and voltage through the circuit is 5A and 12V. A key thing to note is that the max voltage LEDs can consume before damage is termed ‘reverse voltage’. 

