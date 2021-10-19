Lab 4 - Virtual Twin 
======================

.. contents:: :depth: 2

Mini-lecture - TBD
---------------------------------

* Video: Available soon


Lab instructions
-------------------

These instructions assume you are running mac or linux. If you have Windows 10 or lower, I recommend dual-booting linux. If you have Windows 11, try using the Windows Linux Subsystem

Step 1. Set up simulation environment
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
#. Clone the simulator repository ``git clone https://github.com/Nate711/puppersim.git``
#. Go into the repo: ``cd puppersim``
#. Set up the repo with ``python3 setup.py develop``. Use ``python`` if ``python3`` doesn't work.
#. If you read the readme, you'll notice it says to use code from StanfordQuadruped. We're going to use our own fork so skip that step in the readme and instead go to step 2.


Step 2. Set up robot control code
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
#. Open terminal and navigate to a directory where you want to put Pupper-related code
#. Clone the robot control logic repository ``git clone https://github.com/stanfordroboticsclub/StanfordQuadruped``
#. Go into the repo: ``cd StanfordQuadruped``
#. Checkout the dji branch ``git checkout dji``
#. Install dependencies ``pip3 install numpy transforms3d pyserial``. Use ``pip`` if ``pip3`` doesn't work.

Step 3. Try out the simulator
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
#. In the ``puppersim`` folder, run ``python3 puppersim/pupper_server.py``.
#. In another terminal tab/window, go to the ``StanfordQuadruped`` folder and run ``python3 run_djipupper_sim.py``.
#. Check out these keyboard controls: 
    * wasd: left joystick         --> moves robot forward/back left/right.
    * arrow keys: right joystick  --> turns robot left/right
    * q: L1                       --> activates robot
    * e: R1                       --> starts trotting
    * ijkl: d-pad                 --> tilts robot
    * x: X                        --> nothing
    * square: u                   --> nothing
    * triangle: t                 --> nothing
    * circle: c                   --> nothing
#. To activate the robot, press ``q``. To start trotting, press ``e``.
#. Enjoy the simulator!
#. To close the simulator, do not press use the usual close button in the top left of the simulator window. Instead do Ctrl-C in both terminal tabs/windows.

Expected result:

.. figure:: ../_static/lab4/sim.png
    :align: center
    
    Expected simulator window.
    
.. figure:: ../_static/lab4/terminal.png
    :align: center
    
    Expected output from ``python3 run_djipupper_sim.py``.