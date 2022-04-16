Actuator troubleshooting
=================================

DJI C610 motor controller 
----------------------------------

`--> Manual <-- <https://drive.google.com/file/d/1L8oGLUJuZ96MB90XeFtk1E01sL-Uh4BW/view>`_

Motor does not move
^^^^^^^^^^^^^^^^^

* If the motor controller is blinking abnormally or beeping, read page 6 of the manual linked above
* Power cycle the ENTIRE system (including Teensy and motors)
* Turn the motor by hand to see if you can feel if any of the teeth inside the actuator broke
* Check that the cables from the motor to motor controller are not loose or broken

How to calibrate the motor
^^^^^^^^^^^^^^^^^^^^^^^^^^^

#. Arrange the motor so that there is no load on the motor. This means nothing can be preventing the motor from moving, and gravity should not be applying torque to any link attached to the motor.
#. Hold the button on the motor controller down until the motor starts moving
#. Let the motor do its calibration routine
#. Controller should restart and do it's normal green blinking

DJI M2006 motor
----------------------------------
`--> Manual <-- <https://drive.google.com/file/d/1L8oGLUJuZ96MB90XeFtk1E01sL-Uh4BW/view>`_


