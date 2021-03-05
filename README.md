# Nissan-Leaf-BatteryPairing
![BatteryPairing in action](https://i.imgur.com/8NSiohr.png)
Excel VBA macro that generates commands for pairing Nissan LEAF batteries. Works with ZE0 and AZE0 so far. However, I cannot guarantee if this fixes or bricks your car. In a worst case scenario you will have to visit a dealership and get it paired properly with expensive tools.

# What is it for?
Changing the main battery pack in a Nissan Leaf to another one results in the error code P3102, which cause turtle mode with reduced engine power (limp-mode). The file generated will remove the P3102 code and allow for changing main batteries. Note that this is only for direct swaps(24->24 or 30-30kWh), not for battery upgrades(24-30kWh)!

# How to use
1. Read out your new battery ID with LEAFspy Pro BETA. Take an Android phone equipped with Leafspy Pro. Go to the Google playstore, and then to the Leafspy Pro page. Scroll down and apply to become a Beta tester. Then you will get the newest version, which can read out the battery ID. Open the app, and connect to the car. Go to the "ECU Versions" screen from the service menu, and take a screenshot of this page. The screenshot should look like this: https://dalasevrepair.fi/wp-content/uploads/2020/07/ID.png
2. Open the file in this repository with Excel. Enable macros, and enter the BatteryID at the top. Then press the "Generate .log" button and save the .log file to some suitable location.
3. Play back the .log file using the freeware CANrunner (https://www.wapice.com/products/canrunner) and some suitable CAN-device, like a Kvaser/PCAN etc.. Play the messages into the OBD2 port CAR-CAN, primary CAN bus is on the standardized (J2284) connector pins, CAN-L (14) and CAN-H (6).

# Credits
Massive thanks to Сергей Иванов for figuring this out!
