Lab 2 - Safety Dance
====================

.. contents:: :depth: 2

Mini-lecture - Forward Kinematics
------------------------------------

* Video: Available soon

Lab Instructions
------------------

Step 0. Get the starter code
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
#. Get the starter code https://github.com/stanfordroboticsclub/independent-study-lab2

Step 1. Implement and test a forward kinematics function
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
#. Program a function that takes in a BLA::Matrix<3> vector of joint angles and outputs a BLA::Matrix<3> of the corresponding cartesian coordinates of the end-effector.
#. Run the program. The code will test your kinematics code during the setup() function.

Step 2. View cartesian coordinates of end effector
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
#. Start the robot from the base position
#. Print out the cartesian coordinates of the end effector using your forward kinematics function

Step 3. Make a safety box
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
#. Pick a "safety" box -- a virtual box in cartesian coordinates that the robot can operate safely in. For example, -0.1<x<0.1 and -.1<y>0.1 and 0<z<-0.2.
#. Print a warning whenever the robot leaves the safety box.

Step 4. Do the `safety dance <https://youtu.be/AjPau5QYtYs>`_
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
#. Make a function to vibrate the motors (high frequency, low amplitude torque command sinusoid) 
#. Run the function whenever the robot end effector leaves the safety box.

[gif of completed project]