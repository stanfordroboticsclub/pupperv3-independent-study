Lab 4 - Drawbot
================

.. contents:: :depth: 2

Mini-lecture - Inverse Kinematics
----------------------------------

.. raw:: html

    <iframe src="https://stanford195.autodesk360.com/shares/public/SH35dfcQT936092f0e43e4b3d19bbaacc90a?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>
    

*3D illustration of motor angles, directions of positive rotation, and relevant geometry.*


* Video: Available soon


Lab instructions
-------------------

Step 1. Implement and test a inverse kinematics function
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
#. Program a function that takes in a BLA::Matrix<3> vector of the desired cartesian coordinates and outputs a BLA::Matrix<3> of the corresponding joint angles.
#. Test function in Platformio against our test data [todo. figure out platformio tests]

Step 2. Check against forward kinematics
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
#. Come up with some reasonable (i.e. leg configurations you might see on the robot) cartesian end-effector positions
#. Pass those positions to your inverse kinematics function to get joint angles
#. Sanity check the joint angles yourself
#. Pass those joint angles into your forward kinematics function to get predicted cartesian position
#. Check the predicted cartesian position against the cartesian positions you started with
#. If they don't match, but you think your code is correct, think about if your initial cartesian point is compatible with how we derived the inverse kinematics.
#. Remember that for every cartesian point in space, there are two sets of joint angles that will you get there. However, we programmed our inverse kinematics to find a specific one.

Step 3. Program a drawing pattern
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
#. Come up with an easy shape to draw (lines, circles, etc)
#. Program a function that maps time to where, in cartesian coordiantes, the pen should be to draw that shape
#. Dry-run the drawing function by printout out the coordinates and joint angles without commanding the actuators.
#. Do it for real.
