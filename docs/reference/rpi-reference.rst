Raspberry Pi Reference
==========================

SSH and Internet at Stanford
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Note: SSH only works when both the RPi and computer are on the "Stanford network" and in the same building.

#. Connect your RPi to your computer over USB C (both sides) or ethernet cable.
#. SSH into the RPi over the local network ``ssh pi@raspberrypi.local`` :sup:`1`
#. Find the MAC address ``ifconfig``. The MAC address is the hexidemical number in the ether line of the wlan0 section. It looks like 6e:19:c0:ce:a5:22 or similar. [TODO: Insert screenshot].
#. Go to `iprequest.stanford.edu <http://iprequest.stanford.edu/>`_ on your computer
#. On the first page, choose Device Type: Other, Operating System: Linux, Hardware address: the MAC address you found
#. On the second page, choose Other PC, delete what's under Hardware Addresses Wireless and replace with Pi's MAC address.
#. Wait for email that says the device has been accepted.
#. Reboot the Pi ``sudo reboot 0``
#. SSH over cable
#. Connect to the "Stanford" network on the Pi by doing ``sudo raspi-config`` and following options for wifi.
#. Test the connection by doing ``ping google.com`` and checking that bytes are received.
#. SSH into the Pi from your computer via ``ssh pi@[rpi's IP address]`` such as ``ssh pi@192.168.9.69``.

Notes:

:sup:`1` If you cannot SSH over cable, plug a monitor, keyboard, and mouse into the RPi. Then use ``sudo raspi-config`` to enable SSH. Then use ``ifconfig`` to find the ethernet IP address.