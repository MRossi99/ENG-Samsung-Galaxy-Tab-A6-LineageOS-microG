# How to Install LineageOS on Samsung Galaxy Tab A6 (gtaxllte) with MicroG. 
A complete Guide to Install LineageOS 19.1 on Samsung Galaxy Tab A6 with microG for Google services. `(SM-T585)`.
>[!WARNING]
>This guide is for informational purposes only. I take no responsibility if your device bricks or becomes permanently damaged.

Nowadays, Samsung does not support Galaxy Tab a6 anymore. It suffers from heavy slow downs and now most recent apps can't be installed there because the current Android version is outdated. Installing a CustomOS like LineageOS on your tablet can be useful to obtain major improvements, such as better performance, control, privacy, giving it a second life! <br>
<br>
LineageOS supports Samsung galaxy tab A6 unofficially. If you're trying to use BitGApps, NikGApps or MineTheGApps for Google services, you will encounter a lot of tricky troubles. <br>
Follow this guide will help you installing it smoothly.

📥 First of all, download these:
| Name | Link | Note |
| :--- | :--- | :--- |
| **Odin Tool** | [Download](https://odindownload.com/) | Version 3.13.1 |
| **TWRP Recovery** | [Download](https://dl.twrp.me/gtaxllte/) | Last version for SM-T585 |
| **LineageOS 19.1** | [Download](https://xdaforums.com/t/lineageos-19-1-for-sm-t580-gtaxlwifi-sm-t585-gtaxllte-sm-p580-gtanotexlwifi-and-sm-p585-gtanotexllte.4432957/page-95#post-89998855) | For gtaxllte |
| **minMicroG** | [Download](https://github.com/friendlyneighborhoodshane/minmicrog_releases/releases) | Download NoGoolag | <br>

**1. Inject TWRP inside the device**
  - Go to Settings, System, tap on Build Number many times to activate **developer mode**.
  - Open the developer settings and activate **OEM Unlocker** then turn off the tablet.
  - Turn on while pressing `Volume down + Home + Power` simultaneously.
  - Now press `Volume up` and you will be in **Download Mode**.
  - Open **Odin** on your PC. Connect the tablet. You may see a small blue rectangle `[ID:COM]`, if you see it, it's everything fine.
  - Click on **AP** and select the TWRP file (`.tar`).
  - Go to Odin **Options** below and **remove the check** to "Auto Reboot". **(IMPORTANT)**
  - Press **Start** and when you see the green box **PASS** disconnect che cable.
  - Now press simultaneously `Volume down + Home + Power` but when the screen become dark move your fingers to `Volume up + Home + Power` and leave when you see the TWRP menu. <br>
    >In the case you fail the last step, no worries. You can do it again, just enter in download mode, open odin and put the .tar file on AP and inject.<br>
    
**2. Cleaning the device (Wipe)**
  - Now we are inside the TWRP, *swipe* and enter in main menu.
  - Go to **Wipe** and **Format Data** and write `yes` to confirm.
  - Now go back with the "back" button (◄) **(DO NOT CLICK REBOOT)**
  - Click **Advanced Wipe**
  - Select **only** these: `Dalvik / Art Cache`, `System`, `Data`, `Cache`.
  - Swipe to wipe and go back to TWRP main menu. <br>
  
**3. Install LineageOS and MicroG**
  - Connect the tablet to your PC with an USB cable (TWRP will recognize it as external memory unit).
    > Not all cables can transmit Data, some cables just recharge devices and nothing more, pay attention to choose the right cable that can do both.
  - Copy the file `.zip` of **LineageOS** and **microG** inside the tablet memory.
    > It is possible also to transfer files through a MicroSD card, to do that just copy all files there and put it inside your tablet.
  - On your tablet, go to **Install**
  - Select **LineageOS** `.zip` and install.
    > If you don't see any file, just reboot your device, go to TWRP settings and **Recovery**, the device will reboot but it will come back to the TWRP menu.
  - Go back (◄) and install **microG** `.zip` file.
  - Now you can finally click **Reboot System**. <br>
  
**4. How to enable Google Services with MicroG**<br>
*We finally got our tablet with a brand new customOS, but first we have to enable Google Services.*
  - Open the app **MicroG Settings**
  - Click **Check troubles** and check every box, give permissions to microG and go back.
  - Check **Device registration** go back.
  - Check **Cloud messaging** go back.
  - Check **SafetyNet** go back. <br>
  
**5. F-Droid and Aurora Store** <br>
*Now we need to download the apps, first of all download F-Droid (Enable download from external apps).*
  - Open the browser (Purple icon with a white star inside), search for **F-Droid**. must be [this site](https://f-droid.org/it/).
    > **F-Droid** is useful if you need bunch of open source apps, go check it!
  - Enable download from external apps and install it.
  - Open **F-droid** and search for **Aurora Store**
  - Tap **Aurora Store** and select **anonymous mode** to enter inside the store. <br>


> [!NOTE]
> For the major part of Google applications everything will work without any problems, but Youtube App is one of the few that needs other steps. [Here](https://revanced.app/) is the link if you are interested. <br>

Installation is finished, now enjoy your new device with infinite open source possibilities! <br>

**If you wanna go back to last Android version or your device doesn't work**<br>
You can revert everything:<br>
- Go [there](https://samfw.com/firmware/SM-T585) and download the last version of the firmware (select your device language).
- Open Odin and connect your tablet in **Download mode**.
- Inject the files **BL, AP, CP, CSC** in the correct space.
- Press Start.
- Leave it finish and it will reboot automatically with an old version of Android. <br>

>[!TIP]
>This will revert everything, it is useful if TRWP crashes or gives you irreparable errors.

<br>
<details>
  <summary>📂 Pictures of my tablet with LineageOS 19.1</summary>
  <br>
  
[Front](https://github.com/user-attachments/assets/64db537f-bc46-418e-882e-c17f2840ab39)<br>
[Retro](https://github.com/user-attachments/assets/379197c8-02f3-45d4-aad0-f6604dc6da11) <br>
[Operating system info](https://github.com/user-attachments/assets/e0746a80-0084-4130-9b95-f879e4b26636)

</details>
