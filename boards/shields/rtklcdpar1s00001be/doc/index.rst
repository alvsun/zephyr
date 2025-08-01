.. _rtklcdpar1s00001be:

RTKLCDPAR1S00001BE Display
##########################

Overview
********

The Graphics Expansion Board includes a 1024x600 pixel TFT color LCD with a
capacitive touch overlay.

This display uses a 40-pin connector header.

Pins Assignment of the Renesas RTKLCDPAR1S00001BE Display
=========================================================

+-----------------+--------------------------+
| Connector Pin   | Function                 |
+=================+==========================+
| 1               | Display backlight enable |
+-----------------+--------------------------+
| 2               | Touch ctrl I2C SDA       |
+-----------------+--------------------------+
| 3               | External interrupt       |
+-----------------+--------------------------+
| 4               | Touch ctrl I2C SCL       |
+-----------------+--------------------------+
| 6               | Display reset            |
+-----------------+--------------------------+

Hardware Requirements:
**********************

Supported Renesas RA boards: EK-RA8P1

- 1 x RA Board
- 1 x Micro USB cable

Programming
***********

Set ``--shield=rtklcdpar1s00001be`` when you invoke ``west build``. For
example:

.. zephyr-app-commands::
   :zephyr-app: tests/drivers/display/display_read_write
   :board: ek_ra8p1/r7ka8p1kflcac/cm85
   :shield: rtklcdpar1s00001be
   :goals: build
