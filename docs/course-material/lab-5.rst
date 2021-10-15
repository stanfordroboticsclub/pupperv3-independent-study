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

Step 1. Electronic assembly
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
#. Connect motor controllers to motors
#. Calibrate motor controllers 
#. Set IDs on motor controllers. 
#. Label the motor controllers and motor connector cables with the IDs in case you unplug them later.
#. Connect motor controller power cables and CAN connectors to bottom PCB
#. Insert motor controllers into slots
#. Put wire wrap around motor controller cables
#. Zip-tie wire wraps and cables to the motor bulkheads

Step 1. Raspberry Pi assembly
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
#. Solder pin headers to IMU board
#. Plug in IMU into bottom PCB with Sparkfun text facing towards the Teensy USB
#. Screw RPi into electronics bulkhead with M2.5x5 socket head screws such that the Pi is about symmetric on the electronics bulkhead
#. Connect USB C extension cable to Rpi so the cable goes under the RPi
#. Mount electronics bulkhead into the bottom PCB with M3x6 button head screws.
#. Connect RPi to power by using 2-pin cable. Connect one end into pins behind Teensy and other side into Teensy [insert diagram. can easily fry RPi if done incorrectly]
#. Connect RPi camera flex cable into RPi
#. Mount RPi camera with 4x M2x3 screws to front cowling such that flex cable goes up
#. Connect RPi to Teensy using micro usb cable
#. Connect RC receiver to RPi with usb extension cable
#. Screw USB-C connector to the top PCB with M3x6 button head screws
#. Insert XT60 female side (conductor is a circular slot) of XT60 splitter cable into 3D printed power hub. 
#. Connect other female XT60 into the bottom PCB
#. Insert JST-XH extender balance cable into 3D printed power hub.


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


