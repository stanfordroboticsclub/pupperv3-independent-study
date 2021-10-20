Lab 5 - Pupper Assembly
========================

.. contents:: :depth: 2


Lab instructions
-------------------

Step 1. Leg Assembly
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
#. Assemble 2 left legs
#. Assemble 2 right legs

Step 2. Bulkhead assembly
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
#. Insert end stop pins into motor bulkhead
#. Attach 2 motors, one into each side of motor bulkhead
#. Attach left and right legs to the shafts of the motors you just installed

Step 3. Electronic assembly
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
#. Connect motor controllers to motors
#. Calibrate motor controllers 
#. Set IDs on motor controllers. 
#. Label the motor controllers and motor connector cables with the IDs in case you unplug them later.
#. Connect motor controller power cables and CAN connectors to bottom PCB
#. Insert motor controllers into slots
#. Put wire wrap around motor controller cables
#. Zip-tie wire wraps and cables to the motor bulkheads

Step 4. IMU prep
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
#. Break off two 1x6 male header rows.
#. Place them on the *top* side of the IMU board (side with black connectors and the middle chip)
#. Insert the IMU with headers into a breadboard to help you solder the headers to the IMU
#. Solder the headers to the IMU

[insert picture here]

Step 5. Unmounted Raspberry Pi assembly
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
#. Plug in IMU into bottom PCB with Sparkfun text facing towards the Teensy USB
#. Screw RPi into electronics bulkhead with M2.5x5 socket head screws such that the Pi is about centered on the electronics bulkhead
#. Connect USB C extension cable to Rpi
#. Connect RPi camera flex cable into RPi. There's a little grey flap that flips up on the connector that lets you slide the cable in. Flip the flap down to lock the cable in.

Step 6. Mounted Raspberry Pi assembly
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
#. Mount electronics bulkhead into the bottom PCB with two M3x6 button head screws.
#. Connect RPi to power by using 2-pin cable. Connect one end into 5V, GND pins near the Teensy and other side into RPi. Quadruple-check that the 5V and GND pins are going the right places. See diagram below.
#. Mount RPi camera with 4x M2x3 screws to front cowling such that flex cable goes up. The screws thread into the plastic and may be tough to thread.
#. Connect RPi to Teensy using USB A to USB micro cable
#. Connect RC receiver to RPi with ribbon cable usb extension cable. The connectors have gray flaps that slide in/out to lock/unlock the cable.

Step 6.5. Bind RC receiver
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
#. Bind the receiver [TODO: add instructions]

Step 7. Top panel assembly
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
#. Screw the USB-C connector to the top PCB with M3x6 button head screws
#. Insert the XT60 female side (conductor is a circular slot) of XT60 splitter cable into 3D printed power hub. 
#. Connect other female XT60 into the bottom PCB
#. Insert JST-XH extender balance cable into 3D printed power hub.
#. Take the large nut off the power switch and then mount the power switch to the top PCB panel. Then secure the switch by threading on the nut from the bottom of the top panel.
#. Compare your build to the finished robot to see if you missed anything.
#. Verify your build so far with the class instructors and the photos below.

.. figure:: ../_static/rpi-pinout.png
    :align: center
    
    RPi pinout. 

.. figure:: ../_static/djipupper_photos/IMG_0880.jpg
    :align: center
    
    Bulkhead wiring.

.. figure:: ../_static/djipupper_photos/IMG_0881.jpg
    :align: center
    
    Zip-tie close up.

.. figure:: ../_static/djipupper_photos/IMG_0882.jpg
    :align: center
    
    Leg assembly.

.. figure:: ../_static/djipupper_photos/IMG_0883.jpg
    :align: center
    
    Electronics assembly.

.. figure:: ../_static/djipupper_photos/IMG_0884.jpg
    :align: center
    
    Bottom view of top PCB.

.. figure:: ../_static/djipupper_photos/IMG_0885.jpg
    :align: center
    
    Top view of top PCB.


Step 7. Finish hardware assembly
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
#. Put velcro or dual-lock onto the bottom PCB where it says "battery". For now we'll use the power supply to run the robot so you don't have to install the actual battery.
#. Attach the top PCB panel with M3x6 button head screws. 
#. Check again with instructors.
#. Marvel at your work!

Step 8. Flash code onto the Teensy
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
#. ``git clone https://github.com/Nate711/DJIPupperTests.git``
#. Use VSCode PlatformIO to open the DJIPupperTests folder and then upload the code to the Teensy

Step 7. Running the robot
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
#. Get a micro SD card with our software image. Slide it into the Raspberry Pi
#. Power on the robot by hooking up the power supply's female XT60 (slots) to the bottom PCB's male XT60 (prongs).
#. Turn on the RC transmitter by pressing the power button until it turns blue. [TODO verify this is the case]
#. Wait ~30s for the RPi to boot and then flip the the switches [... TODO find out how to flip the switches]
#. Play with the robot! Top right switch flips between trotting and standing. Left/right on the left joystick controls turning. Up/down on the right joystick controls forward/back. Left/right on the right joystick controls strafing left/right.

Step 7. Accessing the robot brain
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
#. Connect the robot to your computer via the top USB-C port on the robot.
#. SSH into the robot with `ssh pi@raspberrypi.local`. Ask for help if this doesn't work.


Resources
-----------

Wiring diagram
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
.. figure:: ../_static/wiring-diagram.png
    :align: center
    
    Wiring diagram.

Work in progress `manual <https://img1.wsimg.com/blobby/go/f1c92971-b8a4-41e7-ae17-e7be47117f4a/downloads/Pupper%202.1%20Manual.pdf?ver=1629132720898>`_.
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
.. .. raw:: html

..     <iframe frameborder=“0” style=“width:100%;height:781px;” src=“https://viewer.diagrams.net/?tags=%7B%7D&highlight=0000ff&edit=_blank&layers=1&nav=1&title=Pupper%20Wiring%20Diagram.drawio#Uhttps%3A%2F%2Fdrive.google.com%2Fuc%3Fid%3D1yEQvr2gm86uTxlCF5FVwHrtBXnDOZnK8%26export%3Ddownload”></iframe>


