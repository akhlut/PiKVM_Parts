PiKVM ATX controller design notes

This design uses RJ45 connectors as they are cheap, compact, and ubiquitous.

The RJ45 pinout (v1.5) uses the T-568B pattern and is as follows:

    PIN_1 : W-O : POWER LED +

    PIN_2 : O-W : POWER LED -

    PIN_3 : W-G : IDE LED -

    PIN_4 : Bl-W : RESET -

    PIN_5 : W-Bl : RESET +

    PIN_6 : G-W : IDE LED +

    PIN_7 : W-Br : POWER +

    PIN_8 : Br-W : POWER -

-----

The GPIO pinout (v1) is as follows:

PORT A

    GPIO 03 - POWER

    GPIO 15 - RESET

    GPIO 04 - POWER LED

    GPIO 14 - IDE LED

PORT B

    GPIO 18 - POWER

    GPIO 27 - RESET

    GPIO 22 - POWER LED

    GPIO 23 - IDE LED

PORT C

    GPIO 10 - POWER

    GPIO 08 - RESET

    GPIO 09 - POWER LED

    GPIO 25 - IDE LED

PORT D

    GPIO 07 - POWER

    GPIO 06 - RESET

    GPIO 12 - POWER LED

    GPIO 05 - IDE LED

---

There is also a port to control an external switch.  A DC barrel jack is provided for connectivity.  There is no polarity, simply Common/Normally Open.  This is useful to control external HDMI/KVM switches.

EXTERNAL CONTROL PORT - GPIO 21
