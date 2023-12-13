# ShenaniganStuff

Random things I find interesting and used myself in the Internet

## Dito Sim Access Point Name
> Experienced On: Rising OS and possibly other Custom ROMs (haven't tested) of Android

  Sometimes a device will not automatically fill out the APN of a SIM Card. The OS may not be able to read the MNC and MCC and some other details, thus, having to manually encode them to the system.

  ##### Solution: 
  1. Go to Access Point Name setting of SIM
  2. Add your internet name (preferably DITO Sim or something along the line)
  3. Set the APN to **internet.dito.ph**
  4. Set the MCC to **515**
  5. Set the MNC to **66**
  6. Set the APN Protocol & APN Roaming Protocol to **IPv4/IPv6**
  7. Set the APN Type to **default**

  ##### Credits
  [**APN Settings**](https://www.apnsettings.org/philippines/dito-ph/) | 
  [**mmutia53**](https://phcorner.net/threads/dito-apn-settings-para-sa-mga-di-makapag-internet-using-dito-simcard.1201155/)


## Flashing Custom ROM using OrangeFox Recovery Project
> Used On: Realme 6 Prro | Model Code: RMX2061

*Assuming you already have bootloader unlocked and other prerequisite stuff*
  
Custom ROMs are great for debloating devices and possibly increasing performance and user experience. There are many great Custom ROMs for Android and maybe even your specific mobile brand. Xiaomi, Asus, Samsung, Poco, and many more have great range of available Custom ROMs for their different models of mobile devices. THe downside of flashing a Custom ROM into your device is the risk of bricking, voiding warranty, preventing proper function of some specific applications.

### Method
1. Download OrangeFox Recovery Project that's fitted for your device model to your internal phone storage
2. Download Custom ROM specifically designed for your device model to your internal phone storage

### If OrangeFox is not installed to device, proceed below
 3. Have a PC. It is a requirement
 4. Download platform-tools from the Android SDK and extract it
 5. Download the OrangeFox Recovery Project to PC and extract the recovery.img file
 6. Open the command prompt in the extracted folder and open your device's fastboot (Commonly by Shut Down > Power Button + Volume Down Button)
 7. For A-only devices, type `fastboot flash recovery /path/to/recovery.img` | For A/B or Virtual A/B devices, type `fastboot boot /path/to/recovery.img` | If not of the mentioned beforehand, it is a special case and the instructions are unclear (Have something to do with manufacturer shits)
 8. Reboot into bootloader mode (May volume keys be of use for navigation and power button for enter key)
 9. Wipe data through the `Trash` icon by ticking `DALVIK cache`, `Metadata`, `Cache`, `System`, and `Vendor` if applicable
 10. Navigate to the OrangeFox Recovery Program zip file and swipe right to install
 11. After rebooting to OrangeFox Recovery Program, navigate to the Custom ROM zip file and swipe right to install
     
### Else, continue below
3. Open your device's fastboot (Commonly by Shut Down > Power Button + Volume Down Button)
4. Reboot into bootloader mode (May volume keys be of use for navigation and power button for enter key)
5. Wipe data through the `Trash` icon by ticking `DALVIK cache`, `Metadata`, `Cache`, `System`, and `Vendor` if applicable
6. Navigate to the Custom ROM zip file and swipe right to install

### Additional Tips
- To check if your dvice supports A/B partition or not, check on Treble Check by KevinT on PlayStore (Haven't used it personally)
- Check out XDA Forums for help and Custom ROMs as well as your device's telegram group chat

### Credits
[**OrangeFox Installation Wiki**](https://wiki.orangefox.tech/en/guides/installing_orangefox) | 
[**XDAForums Official Site**](https://xdaforums.com/) | 
[**Treble Check for Partition**](https://android.gadgethacks.com/how-to/see-if-your-phone-has-a-b-partitions-for-seamless-updates-0299060/) | 
[**Android Partition**](https://source.android.com/docs/core/architecture/bootloader)
  
