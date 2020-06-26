# LineageOS 14.1 for the Huawei P8 Lite (alice)

# Sources needed
### Kernel
This device tree is intended to be used with this kernel repo:

https://github.com/masemoel/kernel_huawei_hi6210sft

branch: 7.x
### Vendor
This device tree is intented to be used with this vendor repo

https://github.com/masemoel/vendor_huawei_alice

branch: 7.x

# How To Prepare the dtree to build

Now you will want to apply the repo patches. These patches modify code in the ROM to work with this device.
Execute the following commands in a linux terminal:
NOTE: you have to run the chmod command if you have some issues on the script 
```bash
cd /home/$USER/los/device/huawei/alice/patches
chmod a+x 'apply.sh'
cd /home/$USER/los
./device/huawei/alice/patches/apply.sh
```
NOTE: If you are going to be offline while you are building, you will need download some prebuilts first.
```bash
cd /home/$USER/los
make fetchprebuilts
```
NOTE: Now you have everything that you need to build LineageOS 14 for your Huawei P8 Lite. 
It may take anywhere from 2 hours to 15 hours depending on system specs for a complete build.
Execute the following commands in a linux terminal:
```bash
cd /home/$USER/los
. build/envsetup.sh
lunch lineage_alice-userdebug
mka bacon
```

Huawei P8Lite detailed specifications:
======================================

Basic         |Spec Sheet
-------------:|:--------------------------------------------------------------------------------------------------------------------------
Network	      | GSM / HSPA / LTE
Launch	      |2015, April
Body	      |143 x 70.6 x 7.7 mm (5.63 x 2.78 x 0.30 in); 131 g (4.62 oz); Dual SIM (Nano-SIM/ Micro-SIM, dual stand-by)
Display	      |IPS LCD capacitive touchscreen, 16M colors; 5.0 inches; 720 x 1280 pixels; Corning Gorilla Glass 3
Platform      |Android OS, v5.0.2 (Lollipop), upgradable to v6.0 (Marshmallow)
Chipset	      |HiSilicon Kirin 620
CPU	      |Octa-core 1.2 GHz Cortex-A53
GPU	      |Mali-450MP4
Memory	      |16 GB, 2 GB RAM; microSD, up to 256 GB (uses SIM 2 slot)
Rear Camera   |13 MP, f/2.0, 27mm, autofocus, dual-LED flash, Geo-tagging, touch focus, face/smile detection, panorama, HDR, 1080p@30fps
Front Camera  |5 MP, 720p
Sound	      |- Active noise cancellation with dedicated mic
WLAN	      |Wi-Fi 802.11 a/b/g/n, WiFi Direct, hotspot
Bluetooth     |v4.0, A2DP, EDR, LE
GPS	      |Yes, with A-GPS, GLONASS
NFC	      |Yes
Radio	      |FM radio
USB	      |microUSB v2.0
Sensors	      |Accelerometer, proximity, compass
Battery	      |Non-removable Li-Ion 2200 mAh battery
Colors 	      |Black, White, Gold


![Huawei P8Lite](http://cdn2.gsmarena.com/vv/pics/huawei/huawei-p8-lite.jpg "Huawei P8Lite")
