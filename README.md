# ShenaniganStuff

Random things I find interesting and used myself in the Internet. 

> [!CAUTION]
> This should not be taken too seriously as the guides listed are just whatever worked for ME and might or might not work for YOU.

With those said, feel free to browse through my compilation!


## Dito Sim Access Point Name
> [!NOTE]
> Experienced on Rising OS and possibly other Custom ROMs (haven't tested) of Android

  Sometimes a device will not automatically fill out the APN of a SIM Card. The OS may not be able to read the MNC and MCC and some other details, thus, having to manually encode them to the system.

  #### Workaround
  1. Go to Access Point Name setting of SIM
  2. Add your internet name (preferably DITO Sim or something along the line)
  3. Set the APN to **internet.dito.ph**
  4. Set the MCC to **515**
  5. Set the MNC to **66**
  6. Set the APN Protocol & APN Roaming Protocol to **IPv4/IPv6**
  7. Set the APN Type to **default**

  #### Credits
  [**APN Settings**](https://www.apnsettings.org/philippines/dito-ph/) | 
  [**mmutia53**](https://phcorner.net/threads/dito-apn-settings-para-sa-mga-di-makapag-internet-using-dito-simcard.1201155/)


## Flashing Custom ROM using OrangeFox Recovery Project
> [!NOTE]
>  Used on Realme 6 Prro | Model Code: RMX2061

*Assuming you already have bootloader unlocked and other prerequisite stuff*
  
Custom ROMs are great for debloating devices and possibly increasing performance and user experience. There are many great Custom ROMs for Android and maybe even your specific mobile brand. Xiaomi, Asus, Samsung, Poco, and many more have great range of available Custom ROMs for their different models of mobile devices. The downside of flashing a Custom ROM into your device is the risk of bricking, voiding warranty, preventing proper function of some specific applications.

### Method
1. Download OrangeFox Recovery Project that's fitted for your device model to your internal phone storage
2. Download Custom ROM specifically designed for your device model to your internal phone storage
3. Open your device's fastboot (Commonly by Shut Down > Power Button + Volume Down Button)
4. Reboot into bootloader mode (May volume keys be of use for navigation and power button for enter key)
5. Wipe data through the `Trash` icon by ticking `DALVIK cache`, `Metadata`, `Cache`, `System`, and `Vendor` if applicable
6. Navigate to the Custom ROM zip file and swipe right to install

> [!IMPORTANT]
> ### If OrangeFox is not installed to device, proceed below
> 3. Have a PC. It is a requirement
> 4. Download platform-tools from the Android SDK and extract it
> 5. Download the OrangeFox Recovery Project to PC and extract the recovery.img file
> 6. Open the command prompt in the extracted folder and open your device's fastboot (Commonly by Shut Down > Power Button + Volume Down Button)
> 7. For A-only devices, type `fastboot flash recovery /path/to/recovery.img` | For A/B or Virtual A/B devices, type `fastboot boot /path/to/recovery.img` | If not of the mentioned beforehand, it  is a special case and the instructions are unclear (Have something to do with manufacturer shits)
> 8. Reboot into bootloader mode (May volume keys be of use for navigation and power button for enter key)
> 9. Wipe data through the `Trash` icon by ticking `DALVIK cache`, `Metadata`, `Cache`, `System`, and `Vendor` if applicable
> 10. Navigate to the OrangeFox Recovery Program zip file and swipe right to install
> 11. After rebooting to OrangeFox Recovery Program, navigate to the Custom ROM zip file and swipe right to install

> [!TIP]
> - To check if your dvice supports A/B partition or not, check on Treble Check by KevinT on PlayStore (Haven't used it personally)
> - Check out XDA Forums for help and Custom ROMs as well as your device's telegram group chat

### Credits
[**OrangeFox Installation Wiki**](https://wiki.orangefox.tech/en/guides/installing_orangefox) | 
[**XDAForums Official Site**](https://xdaforums.com/) | 
[**Treble Check for Partition**](https://android.gadgethacks.com/how-to/see-if-your-phone-has-a-b-partitions-for-seamless-updates-0299060/) | 
[**Android Partition**](https://source.android.com/docs/core/architecture/bootloader)
  
## RealMe Flash Tool
> Used once last 2022 and haven't tried since

Sometimes, you want a specific model of your device. Sometimes, you were dumdum while installing a Custom ROM or rooting your device, thus, bricking your phone. For Realme 6 pro devices, there is a tool for flashing stock ROMs made by the people at XDAForums. The tool is available for Windows 7 and higher. The last release was from 2021 and may be outdated now.

### Credits
[**RFT Tool by Narender Singh and Hikari Calyx**](https://xdaforums.com/t/tool-rft-realme-flash-tool-to-flash-stock-rom-for-unlocked-bootloader.4144969/)

## Spotify Patcher for Windows, Mac, and Linux

Ads are intrusive. Great people made these patchers for spotify in different operating systems to removea ads and improve usage. 

### For Windows | BlockTheSpot

Running the Windows PowerShell command is the easiest option. It does everything for you. Just remember to enable PowerShell to run scripts if you are not able to execute scripts.
To enable PowerShell executing scripts, run the Windows PowerShell as administrator and running `set-executionpolicy remotesigned` to permanently allow PowerShell to run unsigned scripts.
There's also an option from Settings but I forgot how to do it.

PowerShell Command for the script: 
```powershell
[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; Invoke-Expression "& { $(Invoke-WebRequest -UseBasicParsing 'https://raw.githubusercontent.com/mrpond/BlockTheSpot/master/install.ps1') } -UninstallSpotifyStoreEdition -UpdateSpotify" 
```

If you'd like other options of patching your Spotify, check out the main repository

### For Mac and Linux | SpotX-Bash

While I do not have a Mac and thus, can't test if it does run on Mac, I assure that it works smoothly on Linux, specifically Ubuntu. Just install Spotify directly from their website guide and not from the repository store of your Operating System.

Bash command for patching:
```bash
bash <(curl -sSL https://spotx-official.github.io/run.sh)
```

Check out the main repository for more patching options such as blocking spotify update for MacOS, or use the Old or New UI theme of Spotify

### Credits
[**BlockTheSpot**](https://github.com/mrpond/BlockTheSpot) | 
[**SpotX-Bash**](https://github.com/SpotX-Official/SpotX-Bash)

## Microsoft Activation Scripts
Activator for your Windows Operating System and Microsoft Software. Usage is as simple as downloading and running.

> [!NOTE]
> I don't bother booting up my Windows OS to just give out detailed instruction but I assure you that it works perfectly and the methods are easy enough to follow

### For Downloading Windows and Software
[**Massgrave.dev**](https://massgrave.dev/)

### For the script to run
[**MAS**](https://github.com/massgravel/Microsoft-Activation-Scripts)
