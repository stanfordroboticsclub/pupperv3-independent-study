Week 1
=======

.. contents:: :depth: 2

Lecture 1 - Joint Control
---------------------------

* Video: Available soon


Lab 1 - The Worst Surgical Robot
----------------------------------
*Goal: Build two robot arms that mirror each other's motion.*

[Insert GIF of completed robot arms]

Step 0. Setup
^^^^^^^^^^^^^^
Insert photo of required parts: Teensy attached to bottom pcb, power supply, motor, motor controller

Step 1. Connecting hardware
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

#. Plug the M2006's 3-wire power cable and 4-wire ribbon encoder cable into the C610 motor controller.
#. Plug the motor controller's 2-wire power cable into a XT30 port on the Pupper PCB and the 2-wire CAN cable into a smaller CAN port.
#. Plug the Teensy into the socket on the Pupper PCB if it's not already.
#. Plug the power supply or battery into the Pupper PCB's XT60 connector.
#. Plug the Teensy into your laptop via micro USB to USB A/C.
#. Done

[Insert photo of completed setup]

Step 2. Calibrating motor
^^^^^^^^^^^^^^^^^^^^^^^^^^^

Calibration:

#. Hold the motor by the gearbox so that the rotor and shaft can move freely.
#. Press and hold the button on the C610 motor controller until the motor starts moving and release.
#. Wait until the C610 motor controller restarts.

[Insert gif of calibrating and setting id]

Setting controller ID:

#. Press the button on the C610 controller, then a little while later (half second) press the button again. The light should flash green.
#. The light should now flash once every 5 seconds or so. The number of blinks indicates which ID it is. For example two blinks every 5 seconds indicates ID=2.


Step 3. Run bang-bang control
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

#. Open starter code using PlatformIO home page in VSCode
#. Examine where in the code the motor angle and velocity are read. Examine where the motor is commanded.
#. Upload starter code to Teensy
#. Change the bang torque, ie the current command, to (blah).

[Insert gif of uploading code]

Step 4. Write PD position control
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

#. Replace call to bang-bang controller with your PD controller. Use Kp = [blah] and Kd = [blah] to start. Don't forget the negative signs!
#. Upload code to Teensy

[Insert gif of proper PD joint control]

Step 5. Experiment with different parameters
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

#. Keeping Kd constant (blah), experiment with different Kp values from (blah) to (blah)
#. Keeping Kp constant (blah), experiment with different Kd values from (blah) to (blah)
#. See what happens when Kp is too high. Try Kp=[blah] and Kd=[blah].
#. See what happens when Kd is too high. Try Kp=[blah] and Kd=[blah].
#. See what happens when Kd is too low. Try Kp=[blah] and Kd=[blah].

[Insert gif of some instability]

Step 6. Experiment with different loop rates
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

#. Examine where the code is checking if it's time to issue another control update.
#. Change the update rate to 100Hz and use Kp=[blah] and Kd=[blah].
#. Change the update rate to 10Hz with the same Kp and Kd. 

Step 7. Program periodic motion
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

1. Program the motor to track a sinusoidal position, like the psuedocode below. 

.. code-block:: c++

    float time = millis() / 1000.0
    position_target = sin(time)

2. Play around with different frequencies. How high can you raise the frequency before the motor no longer moves as much as you expect? 


Fun fact, the maximum frequency you can go before the motor moves to only 71% of the intended motion is called the bandwidth.


[Insert gif of sinusoidal motion]

Step 8. Connect and calibrate 2 more motors
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

#. Connect power and encoder cables from motors to controllers.
#. Connect power and CAN cables from controllers Pupper PCB

[insert pic of compeleted setup]

Step 9. Program periodic motion for all three motors
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

#. Write two more independent PD controllers for the other two motors
#. Program a similar periodic motion for the other motors. (Or whatever you want)

[insert gif of completed setup]

Step 10. Assemble the three motors into a robot arm!
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

1. Attach the shoulder abductor motor to the base
[insert pic]

2. Attach the base hub to the shoulder abductor motor
[insert pic]

3. Attach the shoulder rotator motor to the base hub
[pic]

4. Attach the upper arm to the shoulder rotator motor
[pic]

5. Attach the elbow motor to the upper arm
[pic]

6. Attach the lower arm to the elbow motor
[pic]

Step 11. Run your code again on the new robot arm
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
[gif]

Step 12. Connect three more motors to use as control dials
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
#. Calibrate and connet three additional motors to the Pupper PCB
#. Set the target positions of the shoulder abductor motor, shoulder rotator motor, and elbow motor to the angle readings of the first, second, and third new motors respectively.

[gif]

Step 13. Assemble the three new motors into a robot arm
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
[pic]

Step 14. Make the robot arms bidirectional!
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
#. Make the leader arm motors also perform position control where the position targets are the angle readings from the former follower arm.
#. Congrats. Play with your robot! Make modifications!

[gif]