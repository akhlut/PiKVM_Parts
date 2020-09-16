PiKVM ATX controller design notes

This design uses RJ45 connectors as they are cheap, compact, and ubiquitous.

The RJ45 pinout (v1) uses the T-568B pattern and is as follows:

    W-O: POWER LED +

    O-W: POWER LED -

    W-G: IDE LED -

    Bl-W: RESET -

    W-Bl: RESET +

    G-W: IDE LED +

    W-Br: POWER +

    Br-W: POWER -

-----

The GPIO pinout (v1) is as follows:

PORT A

    GPIO 03 - POWER

    GPIO 04 - RESET

    GPIO 14 - POWER LED

    GPIO 15 - IDE LED

PORT B

    GPIO 18 - POWER

    GPIO 27 - RESET

    GPIO 22 - POWER LED

    GPIO 23 - IDE LED

PORT C

    GPIO 10 - POWER

    GPIO 09 - RESET

    GPIO 25 - POWER LED

    GPIO 08 - IDE LED

PORT D

    GPIO 07 - POWER

    GPIO 05 - RESET

    GPIO 12 - POWER LED

    GPIO 06 - IDE LED


There is also a port to control an external switch.  A DC barrel jack is provided for connectivity.  There is no polarity, simply Common/Normally Open.  This is useful to control external HDMI/KVM switches.
