# PiKVM_Parts

Parts I've made for the PiKVM Project.  https://github.com/pikvm/pikvm

All parts are UNTESTED as of 9/23/2020

The idea behind this is to extend the core PiKWM and turn it into a 4-port switch.  4-Port HDMI switches are ubiquitous and inexpensive, making them a less than ideal candidate for designing a PCB around.  Given that GPIO pins can be assigned to specific functions it only makes sense to start building out a 4-port USB/ATX controller built on top of PiKVM.  Couple this with a way to mimic a button-press on and HDMI switch and we're in business.  

The USB and ATX PCB's stack on top of one another, minimizing the footprint.  The PCB's extend the width of the Pi, but not the length.  At some point I'll have to design a case.

Everything is drawn in EAGLE as it's the tool that I'm used to.


Questions?  
Ask on the discord server:  https://discord.com/channels/580094191938437144

Ask on the subreddit: https://old.reddit.com/r/pikvm/

Happy soldering!
