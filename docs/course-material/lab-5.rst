Lab 5 - Virtual Twin 
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
#. Clone the simulator repository ``git clone https://github.com/jietan/puppersim.git``
#. Follow the instructions in the **Conda setup link** section and **Getting the code ready** section of the puppersim README.
#. Install dependencies ``pip3 install numpy transforms3d pyserial``. Use ``pip`` if ``pip3`` doesn't work.

Step 2. Try out the simulator
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
#. Follow the instructions in the **Simulating the heuristic controller** section.
#. Check out these keyboard controls: 
    * wasd: --> moves robot forward/back left/right.
    * arrow keys: --> turns robot left/right
    * q: --> activates robot
    * e: --> starts trotting
    * ijkl: --> tilts robot
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


Step 4. Experiment
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
#. Try changing ``self.overlap_time`` (line 52) in ``StanfordQuadruped/djipupper/Config.py``. This controls the amount of time in which all four legs are on the ground for the trot.
#. Try changing ``self.swing_time`` (line 53) in ``StanfordQuadruped/djipupper/Config.py``. This controls the amount of time in which just two legs are on the ground for the trot.
#. Mess around with other things [tbd]