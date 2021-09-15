Week 2
==========

.. contents:: :depth: 2

Lecture 2.1 - Forward Kinematics
------------------------------------

* Video: Available soon

Lab 2.1 - Safety Dance
--------------------------

Step 1. Implement a forward kinematics function
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
#. Program a function that takes in a BLA::Matrix<3> vector of joint angles and outputs a BLA::Matrix<3> of the corresponding cartesian coordinates of the end-effector.
#. Test function in Platformio against our test data [todo. figure out platformio tests]
#. Set torque command to robot arm to zero and print out cartesian angles of the end effector.
#. Pick a "safety" box -- a virtual box in cartesian coordinates that the robot can operate safely in. For example, -0.1<x<0.1 and -.1<y>0.1 and 0<z<-0.2.
#. Program the robot arm to vibrate (high frequency, low amplitude torque command sinusoid) [todo, figure out frequency and amplitude] when the robot arm escapes the safety box.

[gif of completed project]

Lecture 2.2 - Inverse Kinematics
---------------------------------

* Video: Available soon

Lab 2.2 - Drawbot
------------------