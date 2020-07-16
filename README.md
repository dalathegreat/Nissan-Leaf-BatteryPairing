# Nissan-Leaf-BatteryPairing
Commands for pairing batteries. Only works for 24->24kWh ZE0 (2011-2013) car & battery. Totally untested, I cannot guarantee if this fixes or bricks your car. In a worst case scenario you will have to visit a dealership and get it paired properly.
## EDIT: Commands seem to not work, seed-key wrong?

# What is it for?
Changing the main battery pack in a Nissan Leaf to another one results in the error code P3102, which cause turtle mode with reduced engine power (limp-mode). If this works then it should remove the P3102 code and allow for changing main batteries. 

# How to use
Play back the commands.log messages using the freeware CANrunner (https://www.wapice.com/products/canrunner) and some suitable CAN-device, like a Kvaser. Play the messages into the OBD2 port CAR-CAN, primary CAN bus is on the standardized (J2284) connector pins, CAN-L (14) and CAN-H (6).

# Did it work?
Did it mess up your car? Did it remove the P3102? Please report back, and note that this is only for ZE0 (2011-2013) Leafs at the time. I cannot be held responsible for any damages caused by this, this is used fully on at your own risk!
## One user tested this, reported that the commands did nothing. The user theoretized that a seed-key might be wrong, and that is causing the commands to be ignored. He had access to other tool that could reset BMS stats, and recorded those and tried to play them back without success. So there is something missing when replaying commands.
