# MagicTrackPad2_Windows_Precision_Drivers
Apple's Official Windows 10/11 Precision Trackpad Drivers for both USB-C and Lightning Magic Trackpad 2 models. 
Extracted from Bootcamp Driver packages. 
# Connection
USB/Bluetooth

# Installation Steps
1. Connect the Magic Trackpad with Bluetooth (NOT WITH CABLE).  
2. Go to `Device Manager`  
3. Open the `Human Interfaces Devices` section -> find the listing for `Bluetooth HID Device` -> right click and select `Properties` -> `Details` tab -> select `Hardware Ids` property -> ensure the value starts with `BTHENUM\{00001124` as there may be multiple entries with the same name of Bluetooth HID Device  
4. Go to `Driver` tab in the properties window -> click `Update Driver` -> `Browse my computer for drivers` -> `Let me pick from a list of available drivers on my computer` -> click `Have disk` -> select the  `ApplePrecisionTrackpadBluetooth.inf` file from `ApplePrecisionTrackpadBluetooth` folder and click `OK` -> click `Next`  
5. Wait for installation
6. Now your Trackpad should work with Precision menu option in Windows Settings.

## Important!
The driver has a bug of reconnection failure on latest Windows 10/11 if you remove the Magic Trackpad in Bluetooth Settings, you'd better follow the steps in this [issue](https://github.com/lc700x/MagicTrackPad2_Windows_Precision_Drivers/issues/1)
