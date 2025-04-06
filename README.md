# Samsung Galaxy A12s (sm-a127f/ds)

##### A simple guide to root and install a GSI in the sm-a127f/ds devices and many more customizations

> [!warning]  
> **I am not responsible for bricked or broken devices!** You are doing this out of your free will!!  
> **All Data will be Lost** - You are responsible for your data

## Index

- [Prerequisites](#prerequisites)
- [Required Files](#files)
- [Rooting Process](#rooting)
  - [Step 1: Unlocking the OEM](#step-1-unlocking-the-oem)
  - [Step 2: Flashing Rooted AP](#step-2-flashing-rooted-ap)
- [Additional Guides](#additions)
  - [Rooting AP Using Magisk](#rooting-ap-using-magisk)
- [Installing GSI](#installing-gsi)
  - [Flashing GSI](#step-2--flashing-the-gsi)
  - [TWRP Setup](#step-3--twrp-setup)
- [About](#about)
  - [Credits](#credits)

---

## Prerequisites

- A Samsung A12s device
- A qualified USB cable
- A PC preferably Windows
- A lot of patience and a working brain

## Files

| File         | Download Link                                                                                                                  |
| ------------ | ------------------------------------------------------------------------------------------------------------------------------ |
| Stock ROM    | [Download](https://samfw.com/firmware/SM-A127F)                                                                                |
| Rooted AP    | [Download](https://sourceforge.net/projects/g-flame-oss-file-host/files/sm-a127f/lineageos-20.tar/download)                    |
| Odin Patched | [Download](https://forum.xda-developers.com/attachments/odin3-v3-14-1_3b_patched-zip.5158507/)                                 |
| TWRP         | [Download](https://github.com/edward0181/android_device_samsung_a12/releases/download/twrp-3.6.1_11-1/twrp-3.6.1_11-1-a12.img) |

### GSI Files

| File                    | Download Link                                                                                                                                     |
| ----------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------- |
| Lineage OS              | [Download](#)(https://sourceforge.net/projects/g-flame-oss-file-host/files/sm-a127f/lineageos-20.tar/download) (Includes TWRP and patched VBmeta) |
| Kernel                  | [Download](/files/kernel/kernel-perm-ksu.zip)                                                                                                     |
| Magisk APK              | [Download](/files/apks/magisk.apk)                                                                                                                |
| Touch Fix               | [Download](/files/magisk-modules/Touch-fix.zip)                                                                                                   |
| GApps                   | [Download](/files/magisk-modules/MagiskGApps.zip)                                                                                                 |
| Device ID               | [Download](/files/apks/deviceid.apk)                                                                                                              |
| GSI Customization Files | [Download](/customization/)                                                                                                                       |

---

## Rooting

> [!CAUTION] > **All data will be erased during this process. Back up any important data before proceeding.**

For those who want the latest Magisk, go to the [Rooting AP Using Magisk](#rooting-ap-using-magisk) section.

### Step 1: Unlocking the OEM

For a better visual guide, check [THIS VIDEO TUTORIAL](https://www.youtube.com/watch?v=8Y0BKZXChiA).

1. Go to **Settings** > **About phone** > tap the build number 5-7 times until Developer options are unlocked
2. Go back to Settings main page and scroll down until you see **Developer options**
3. Enable the **OEM unlock** option and shutdown your phone
4. On your PC, download the files from the [Files section](#files)
5. Extract the Odin file and open it
6. Connect the USB cable to the PC (**_DO NOT CONNECT TO PHONE YET_**)
7. Press the **Volume Up** and **Volume Down** buttons simultaneously and connect the cable to the phone
8. Hold the **Volume Up** button when you see this screen:

   <div align="center">
     <img src="./files/assets/warning_svb.jpg" width="300" style="border: 1px solid #ddd; border-radius: 4px; padding: 5px; margin: 10px 0;"/>
     <p><i>Warning Screen</i></p>
   </div>

9. Press **Volume Up** to fully unlock the OEM

   <div align="center">
     <img src="./files/assets/device_unlock.jpg" width="300" style="border: 1px solid #ddd; border-radius: 4px; padding: 5px; margin: 10px 0;"/>
     <p><i>Device Unlock Screen</i></p>
   </div>

10. Disconnect the cable from the phone
11. Your phone will shutdown and reset itself. Power off your phone.
12. Press the **Volume Up** and **Volume Down** buttons simultaneously and connect the cable to the phone
13. Press **Volume Up** when prompted

    <div align="center">
      <img src="./files/assets/warning.jpg" width="300" style="border: 1px solid #ddd; border-radius: 4px; padding: 5px; margin: 10px 0;"/>
      <p><i>Warning Prompt</i></p>
    </div>

14. You will be greeted with this download mode screen:

    <div align="center">
      <img src="./files/assets/download.jpg" width="300" style="border: 1px solid #ddd; border-radius: 4px; padding: 5px; margin: 10px 0;"/>
      <p><i>Download Mode</i></p>
    </div>

### Step 2: Flashing Rooted AP

1. Download the rooted AP from the [Files section](#files) or follow the [Rooting AP Using Magisk](#rooting-ap-using-magisk) guide
2. Open Odin on your PC
3. Apply these options in the Options tab:

   <div align="center">
     <img src="./files/assets/odin-options.jpg" width="400" style="border: 1px solid #ddd; border-radius: 4px; padding: 5px; margin: 10px 0;"/>
     <p><i>Odin Options Configuration</i></p>
   </div>

4. Select the AP button and browse for the downloaded .tar file:

   <div align="center">
     <img src="./files/assets/odin-ap.jpg" width="400" style="border: 1px solid #ddd; border-radius: 4px; padding: 5px; margin: 10px 0;"/>
     <p><i>Selecting AP File in Odin</i></p>
   </div>

5. Click Start:

   <div align="center">
     <img src="./files/assets/odin-ap-selected.jpg" width="400" style="border: 1px solid #ddd; border-radius: 4px; padding: 5px; margin: 10px 0;"/>
     <p><i>Odin with AP File Selected</i></p>
   </div>

6. Wait for the process to complete. You'll see a "PASS!" message when successful.
7. Hold **Volume Down** & **Power Button** to Reboot your phone !

   <div align="center">
     <p><i>Viola Rooting complete!!</i></p>
   </div>

---

## Installing GSI

> [!important]
> Download required files [here](#gsi-files) and put it in an sd card and put inside the phone.

### Step 1: Booting into Download mode..

1. Your phone will shutdown and reset itself. Power off your phone.
2. Press the **Volume Up** and **Volume Down** buttons simultaneously and connect the cable to the phone
3. Press **Volume Up** when prompted

### Step 2 : Flashing the GSI..

1. Download the Lineage OS GSI [here](#gsi-files)
2. Open Odin on your PC
3. Apply these options in the Options tab:

   <div align="center">
     <img src="./files/assets/odin-options.jpg" width="400" style="border: 1px solid #ddd; border-radius: 4px; padding: 5px; margin: 10px 0;"/>
     <p><i>Odin Options Configuration</i></p>
   </div>

4. then in the AP slot insert the downloaded lineage-os-20.tar file.
   <div align="center">
     <img src="./files/assets/odin-ap-gsi-selected.jpg" width="400" style="border: 1px solid #ddd; border-radius: 4px; padding: 5px; margin: 10px 0;"/>
     <p><i>Odin GSI Install Config...</i></p>
   </div>
5. click start
6. Now Hold **Volume Down** & **Power Button** to Reboot your phone and when the screen goes blank hold the **Volume Up** and press the **Power Button** once and hold the **Volume Up** until TWRP boots up

### Step 3 : Twrp setup

1. open twrp and select **wipe**
   <div align="center">
     <img src="./files/assets/twrp/home.png" width="400" style="border: 1px solid #ddd; border-radius: 4px; padding: 5px; margin: 10px 0;"/>
     <p><i>Home</i></p>
   </div>
2. Select **Advanced wipe**
   <div align="center">
     <img src="./files/assets/twrp/wipe.png" width="400" style="border: 1px solid #ddd; border-radius: 4px; padding: 5px; margin: 10px 0;"/>
     <p><i>Wipe</i></p>
   </div>
3. select **Data** and click **Repair or change File system**
   <div align="center">
     <img src="./files/assets/twrp/data-select-wipe.png" width="400" style="border: 1px solid #ddd; border-radius: 4px; padding: 5px; margin: 10px 0;"/>
     <p><i>Data</i></p>
   </div>
4. select **Change File system**
   <div align="center">
     <img src="./files/assets/twrp/data-advanced.png" width="400" style="border: 1px solid #ddd; border-radius: 4px; padding: 5px; margin: 10px 0;"/>
     <p><i>EXT4</i></p>
   </div>
5. select **EXT4** and swipe
   <div align="center">
     <img src="./files/assets/twrp/format-ext4-confirm.png" width="400" style="border: 1px solid #ddd; border-radius: 4px; padding: 5px; margin: 10px 0;"/>
     <p><i>Confirm</i></p>
   </div>
6. Go **Home** and select **Advanced**
   <div align="center">
     <img src="./files/assets/twrp/advanced.png" width="400" style="border: 1px solid #ddd; border-radius: 4px; padding: 5px; margin: 10px 0;"/>
     <p><i>Advanced Options</i></p>
   </div>
7. Now select **Terminal** and the type the following **multidisabler && multidisabler** and hit enter
   <div align="center">
     <img src="./files/assets/twrp/terminal.png" width="400" style="border: 1px solid #ddd; border-radius: 4px; padding: 5px; margin: 10px 0;"/>
     <p><i>Terminal</i></p>
   </div>
8. Now go **home** and select **Wipe** > **Advanced wipe** > **Data** > **repair or change filesystem** > **change filesystem** > **F2fs** > **Swipe**
   <div align="center">
     <img src="./files/assets/twrp/format-f2fs-confirm.png" width="400" style="border: 1px solid #ddd; border-radius: 4px; padding: 5px; margin: 10px 0;"/>
     <p><i>Format to F2fs</i></p>
   </div>
9. Now go home and select **Install** and and **Select Storage** and choose **SD card** or **Micro SD** and select **kernel-perm-ksu.zip**
   <div align="center">
     <img src="./files/assets/twrp/install.png" width="400" style="border: 1px solid #ddd; border-radius: 4px; padding: 5px; margin: 10px 0;"/>
     <p><i>Install kernel</i></p>
   </div>
10. install the kernel **Swipe**
<div align="center">
  <img src="./files/assets/twrp/install-confirm.png" width="400" style="border: 1px solid #ddd; border-radius: 4px; padding: 5px; margin: 10px 0;"/>
  <p><i>Confirm install</i></p>
</div>

11. Now go to **home** > **Wipe > **Advanced Wipe** > select **cache** & **Dalivic and Art cache** > **Swipe\*\*
<div align="center">
  <img src="./files/assets/twrp/data-select-cache.png" width="400" style="border: 1px solid #ddd; border-radius: 4px; padding: 5px; margin: 10px 0;"/>
  <p><i>Confirm install</i></p>
</div>

12. Now go **home** > **Reboot** > **System**
<div align="center">
  <img src="./files/assets/twrp/reboot.png" width="400" style="border: 1px solid #ddd; border-radius: 4px; padding: 5px; margin: 10px 0;"/>
  <p><i>Confirm install</i></p>
</div>

   <div align="center">
     <p><i>Viola GSI install complete!!</i></p>
   </div>

---

## Additions

### Rooting AP Using Magisk

If you prefer using the latest version of Magisk instead of the pre-rooted AP:

1. Download the Magisk app from [GitHub Releases](https://github.com/topjohnwu/Magisk/releases)
2. Download the stock firmware [here](/files/apks/magisk.apk) according to your country type
3. Extract the stock firmware to a folder on your PC
4. Open Magisk app on another Android device (or emulator)
5. Tap on the **Install** button
6. Select **"Select and patch a file"**
7. In the browser, navigate to the extracted folder and select the AP file
8. Let Magisk patch the file (this may take several minutes)
9. When complete, download the resultant .tar file to your PC
10. Continue with the [Rooting guide's Step 2](#step-2-flashing-rooted-ap) using this patched file

---

<div align="center">

### About

This Guide was Created by **[g-flame](https://github.com/g-flame)** for the **[g-flame-oss](https://github.com/g-flame-oss)**
Check out my other projects **[here](https://github.com/orgs/g-flame-oss/repositories)**
please Star this guide if you like it or found it useful

## Credits

**[physwizz](https://github.com/physwizz)** for the Kernel and Twrp and the scattered Guides for the Exynos 850 chipset and their **[Telegram Group](https://t.me/a127f_res)** for their Guidance..

This **[Guide](<https://github.com/phhusson/treble_experimentations/wiki/Samsung-Galaxy-A12s-(Exynos-850)>)** by **[Mizumo-prjkt](https://github.com/Mizumo-prjkt)** For the Super.img GSI creation

</div>
