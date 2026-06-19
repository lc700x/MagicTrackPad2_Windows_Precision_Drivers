# MagicTrackPad2_Windows_Precision_Drivers
Apple's Official Windows 10/11 Precision Trackpad Drivers for both USB-C and Lightning Magic Trackpad 2 models. 
Extracted from Bootcamp Driver packages. 
# Connection
USB/Bluetooth

# Installation Steps
1. Unpack the ZIP file corresponding to your model:
   * Magic Trackpad 1st gen: [`Old_AppleWirelessTrackpad.zip`](Old_AppleWirelessTrackpad.zip)
   * Magic Trackpad 2nd gen with Lightning port: [`ApplePrecisionTrackpad_amd64(Lightning Only).zip`](ApplePrecisionTrackpad_amd64(Lightning%20Only).zip)
   * Magic Trackpad 2nd gen with USB-C port: [`ApplePrecisionTrackpad_amd64(USB-C).zip`](ApplePrecisionTrackpad_amd64(USB-C).zip)
2. Connect the Magic Trackpad with Bluetooth (NOT WITH CABLE).  
3. Go to `Device Manager`  
4. Open the `Human Interfaces Devices` section -> find the listing for `Bluetooth HID Device` -> right click and select `Properties` -> `Details` tab -> select `Hardware Ids` property -> ensure the value starts with `BTHENUM\{00001124` as there may be multiple entries with the same name of Bluetooth HID Device  
5. Go to `Driver` tab in the properties window -> click `Update Driver` -> `Browse my computer for drivers` -> `Let me pick from a list of available drivers on my computer` -> click `Have disk` -> select the  `ApplePrecisionTrackpadBluetooth.inf` file from `ApplePrecisionTrackpadBluetooth` folder you unpacked and click `OK` -> click `Next`  
6. Wait for installation
7. Now your Trackpad should work with Precision menu option in Windows Settings.

## Important!
- The driver has a bug of reconnection failure on latest Windows 10/11 if you remove the Magic Trackpad in Bluetooth Settings, you'd better follow the steps in this [issue](https://github.com/lc700x/MagicTrackPad2_Windows_Precision_Drivers/issues/1)
