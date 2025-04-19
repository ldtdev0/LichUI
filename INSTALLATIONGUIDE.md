# Installation guide

> [!CAUTION]
> **Read very carefully!** <br/>
> **Installing a custom ROM will erase your data, so back it up!**

## Prerequisites
1) Install <kbd> [Samsung USB driver](https://developer.samsung.com/android-usb-driver) </kbd>, <kbd> [Odin](https://odindownloader.com/download/odin3-v3-14-4) </kbd> and download <kbd> [LichUI](releases/latest/) </kbd> to your PC 
2) If you have `EGY` csc `A546EXXSBCYA2` (for E model) and `EUX` csc `A546BXXSBCYB1` (for B model) - **skip 3, 13, 14, 15 points** 
3) If you haven't `EGY` csc for E model and `EUX` csc for B model - download and unpack your stock system to PC: 
- <kbd> [B model: A546BXXSBCYB1, CSC EUX](https://samfw.com/firmware/SM-A546B/EUX/A546BXXSBCYB1) </kbd>
- <kbd> [E model: A546EXXSBCYA2, CSC EGY](https://samfw.com/firmware/SM-A546E/EGY/A546EXXSBCYA2) </kbd>
4) Download last <kbd> [OrangeFox Recovery](https://github.com/Vaz15k/android_device_samsung_a54x/releases/tag/2024-12-08) </kbd> to your PC for your phone model
5) Download `vbmeta_patched`:
- <kbd> [B model](https://github.com/Vaz15k/proprietary_vendor_samsung_a54x/releases/tag/A546BXXSBCYB1_OXM) </kbd>
- <kbd> [E model](https://github.com/Vaz15k/proprietary_vendor_samsung_a54x/releases/tag/A546EXXSBCYA2_OJM) </kbd>
6) Unlock OEM and Download mode (You need to press `Build number` several times and сlick `OEM unlocking` in developer settings)
7) Turn off your Samsung and connect cable to PC. After connecting you see the charging state
> [!WARNING]
> **Do not disconnect the cable before the 31th point!**

## Steps
8) Press `Volume Up` + `Volume Down` at the same time and hold it before enabling Download mode
9) If the bootloader asks you to unlock it, hold down the `Volume Up` button for any seconds (before unlocking)
10) After this - skip start settings if the phone booted and resets the settings
11) Unpack and open Odin
12) Turn off your phone and repeat the 8th point
13) Go to Odin, find your unpacked stock system and install `BL` to `BL`, `AP` to `AP`, `CP` to `CP`, `CSC` to `CSC` (check stock files name)
14) After installation, your phone will boot to system. Skip start settings. After this - turn off your phone and repeat the 8th point
> [!WARNING]
> **Do not close Odin!**

15) Click `RESET` in Odin
16) Click to `AP` - find your OrangeFox Recovery in PC and click to it
17) Click to `USERDATA` - find your `vbmeta_patched` in PC and click to it
18) Click to `Options` in Odin and disable `Auto Reboot`, `Nand Erase`, `Re-Partition`
19) Click `START`
20) After installation (you'll see "PASS"), press `Power Button` + `Volume Down` at the same time and hold it before the black screen
21) When you see the black screen - fast press `Power Button` + `Volume Up` at the same time and hold it before the phone shows OrangeFox Recovery
22) In OrangeFox click the basket button - click `format data` - write `yes`
23) **Don't click `Reboot`** and copy `LICHUI_4.0.x_a54x.zip` from PC to your phone's internal storage (if your PC sees your internal storage while phone is in recovery, **just skip 24-27 points**)
<br/>

24) Click `Reboot system` and skip start settings again 
25) After skipping - allow data transfer in the pop-up window on the phone 
26) Copy `LICHUI_4.0.x_a54x.zip` from PC to your phone's internal storage
27) After copying turn off your phone and press `Power Button` + `Volume Up` at the same time and hold it before it shows OrangeFox Recovery
<br/>

28) In recovery click the first button from the bottom left
29) Find your `LICHUI_4.0.x_a54x.zip file`, click to it and swipe to right for install
30) After installation - repeat the 22th point and click `Reboot system`
<br/>

31) **Done!**

## Credits
Installation guide by **[Arseniy](https://t.me/Arsenybespomestnov)** and **[ldt](mailto:ldr9660@gmail.com)**
