![crDroid](https://camo.githubusercontent.com/66222527ac34ef135635339adaa9352a479ba331/68747470733a2f2f637264726f69642e6e65742f696d672f6c6f676f2e706e67 "crDroid")

crDroid 3.8.9 for the Huawei P8 Lite (alice)

# Sources needed
--> Kernel <--

This device tree is intended to be used with this kernel repo:

https://github.com/masemoel/kernel_huawei_hi6210sft

branch: crDroid-N

--> Vendor <--

This device tree is intented to be used with this vendor repo:

https://github.com/masemoel/vendor_huawei_alice

branch: crDroid-N

--> Manifest <--

I built crDroid with this manifest:

https://github.com/masemoel/local_manifests/blob/master/alice_nougat.xml

It has all the necessary repos for alice.

# How to build
Download crDroid's source and alice's required stuff (see my attached manifest). Then go to the source folder and run:

```bash
. build/envsetup.sh
lunch lineage_alice-userdebug
make bacon
```
NOTE: patches will automatically be applied when running envsetup.sh .

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
