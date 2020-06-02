# Nissan-Leaf-BatteryPairing
Commands for pairing batteries. Totally untested, I cannot guarantee if this fixes or bricks your car.

# What is it for?
Changing the main battery pack in a Nissan Leaf to another one results in the error code P3102, which cause turtle mode with reduced engine power (limp-mode). If this works then it should remove the P3102 code and allow for changing main batteries. 

# How to use
Play back the messages using CANrunner and a suitable CAN-device, like a Kvaser. Play the messages into the OBD2 port CAR-CAN, primary CAN bus is on the standardized (J2284) connector pins, CAN-L (14) and CAN-H (6).

# Did it work?
Did it mess up your car? Did it remove the P3102? Please report back, and note that this is only for ZE0 (2011-2013) Leafs at the time.
