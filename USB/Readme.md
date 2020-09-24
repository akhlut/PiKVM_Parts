PiKVM USB splitter design notes

AS OF 09232020 THIS DESIGN IS COMPLETE BUT UNTESTED!!!

This design uses Analog Devices ADUM3160 iCouplers to provide galvanic isolation between the OTG USB and the (4) external USB ports.

The GPIO pinout (v1.6) is as follows:

PORT A

    GPIO 17

PORT B

    GPIO 24

PORT C

    GPIO 11

PORT D

    GPIO 13

The OTG port can be switched to Ports A-D by holding GPIO HIGH.  

The OTG port does NOT supply power to the Raspberry Pi!  

Power the Pi by either: 

(1) Use the POWER-IN Port on the PCB to supply 5V to the PCB and Pi via the GPIO header

OR

(2) Use a POE hat to power the PI and use jumper cables to power the PCB @ AUX_PWR header

NEVER USE BOTH POWER OPTIONS AT ONCE!

