# Dell Latitude-7400-Hackintosh

## Disclaimer
- No testing is being done! 
- I am not responsible for your problems!
- If you destroy your hardware or software it is your problem!


## Compatible MacOS Versions
- Sonoma (Could be unstable)
- Ventura
- Monterey
- BigSur

## My System
- Intel Core i7-8665U
- 16GB DDR4 RAM
- Intel UHD 620 Graphics
- Toshiba KIOXIA 512GB SSD
- Intel Wireless-AC 9560

## Confirmed Issues
Open issue for it to be listed

- Airport Stuff (Airdrop, Sidecar, etc.)
- Sometimes Bluetooth (Sonoma is good)
- Bootchime
- HDMI
- WWAN (SIM)
- GPS
- Microphone

# Install Guide

## Creating the USB
- Download the EFI for your macOS Version, unzip and extract EFI Folder
- [Generate your SMBIOS](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/coffee-lake.html#platforminfo) (use MacBookPro15,1)
- [Create the USB](https://dortania.github.io/OpenCore-Install-Guide/installer-guide/#creating-the-usb)

## BIOS Setup
- Boot into BIOS using the F2 Key
- Reset to Default BIOS
- Reboot into BIOS
-------------------------------------------------------------------
- SATA Operations - AHCI

- Secure Boot Enable - Disabled
- Expert Key Management - unchecked
  
- Intel SGX Enable - Enabled
- Enclave Memory Size - 64MB

## Boot
- Boot into Boot-Menu using F12 Key
- Select USB
- If it reboots try again
- When in Opencore Menu press Space Key
- Select the orange Option (dmg)

## Install
- Connect to WIFI or LAN
-------------------------------------------------------------------
- Open Disk Utility
- Select "Show all devices" under View
- Select your disk
- Click erase then select "APFS" and type a name
-------------------------------------------------------------------
If you want to dual boot:

- Click on Partition
- Create a Partition for each OS
- Save
-------------------------------------------------------------------
- Exit Disk Utility
-------------------------------------------------------------------
- Open Reinstall macOS
- Go throught
- Wait
-------------------------------------------------------------------
- If succesful it will reboot sometimes
- Select macOS Installer if it reboots to Opencore Menu

## Post-Install
- Reboot, press space in Opencore menu and reset nvram
- Configure macOS as you like
- [Grab Opencore off the USB](https://dortania.github.io/OpenCore-Post-Install/universal/oc2hdd.html#grabbing-opencore-off-the-usb)
- Have fun!

# Extras

## Updating

- Just do this with the new EFI: [Grabbing Opencore off the USB](https://dortania.github.io/OpenCore-Post-Install/universal/oc2hdd.html#grabbing-opencore-off-the-usb)
- If you upgrade to new macOS Version replace EFI before you reboot!

## Dual Boot with Linux/Windows

- Install your other OS on an empty Partition you created during Install 

## Editing the EFI
- Use [Opencore Install Guide](https://dortania.github.io/OpenCore-Install-Guide/) or other sites
- You can also use [OCAuxiliaryTools](https://github.com/ic005k/OCAuxiliaryTools) for simpler editing

## Contributing
Follow the [Guidelines](https://github.com/toschief/Dell-Latitude-7400-Hackintosh/blob/4308263a2a95329e4da731433a0454f5ce33eca4/CONTRIBUTING.md)

## Credits
- toschief for EFI and Guide
- dortina for Opencore and Opencore Guide
- OpenIntelWireless for Intel Wifi and Bluetooth
- Apple for macOS
- All other file creators for their great work on hardware support
