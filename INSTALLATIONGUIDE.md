# Installation guide

> [!CAUTION]
> **Read very carefully!**

## Prerequisites
1) Install <kbd> [Samsung USB driver](https://developer.samsung.com/android-usb-driver) </kbd>, <kbd> [Odin](https://odindownloader.com/download/odin3-v3-14-4) </kbd> and download <kbd> [LichUI](releases/latest/) </kbd> to your PC
2) If you have `EGY` csc `A546EXXSBCYA2` (for E model) and `EUX` csc `A546BXXSBCYB1` (for B model) - **skip 3, 13, 14,15 points**
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
8 - Press Volume Up + Volume Down at the same time and hold it before enable download mode
9 - If the bootloader asks you to unlock him, hold down the Volume Up button for any seconds (before unlocking)
10 - Good boy - you unlock bootloader! (after this - skip start settings if the phone was boot and resets the settings) 11 - Unpack and open Odin 12 - Turn off phone and repeat 8th point
13 - After download firmware, go to Odin, find your unpacked stock system and install BL to BL, AP to AP, CP to CP, CSC to CSC (Check stock files name for install)
14 - After install, your phone will boot to system. You need to skip start settings. After this turn off phone and repeat 8th point (Don't close Odin)
15 - Click "RESET" in Odin
16 - Click to AP - find your OrangeFox recovery in PC and click to this
17 - Click to USERDATA - find your patched_vbmeta in PC and click to this
18 - Click to "options" in Odin and disable Auto Reboot, Nand Erase, Re-Partition
19 - Click "START"
20 - After install (you'll see PASS) press Power Button + Volume Down at the same time and hold it before the black screen
21 - When you see black screen - fast press Power Button + Volume Up at the same time and hold it before show OrangeFox recovery
22 - In OrangeFox click to basket button - click "format data" - write "yes"
23 - Don't click "Reboot" and copy LICHUI_4.0.3_a54x.zip from PC to your phone in internal storage (If your PC see your internal storage while phone is in recovery, just skip 24-27 points ! ! !)
24 - Click "reboot" - "system" and skip start settings again (If your PC does not see your internal storage while phone is in recovery)
25 - After skip - allow data transfer in the pop-up window on the phone 
26 - Copy LICHUI_4.0.3_a54x.zip from PC to your internal storage of the phone
27 - After copy turn off phone and press Power Button + Volume Up at the same time and hold it before show OrangeFox recovery
28 - In recovery click the first button is from the bottom left
29 - Find your LICHUI_4.0.3_a54x.zip file, click to him and swipe to right for install
30 - After install - repeat 22 point and click "reboot" - "system"
31 - Done!
