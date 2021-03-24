# Lenovo-G50-80-OC
# Introduction
This is the EFI folder for installing hackintosh in Lenovo G50-80 80E5. I made it from EFI Maker and the rest by myself.
# Lenovo G50-80 Basic Specs:
Type: Laptop

CPU: Intel i7-5500U (4) @ 2.40GHz 

GPU: Intel HD Graphics 5500 

RAM: DDR3 8GB (1600MHz)

Audio: Conxeant SmartAudio HD

Ethernet: Realtek RTL8168GU/8111GU PCI Express Gigabit Ethernet

Wifi: Qualcomm Atheros AR9565 Wireless Network Adapter

Bluetooth: Qualcomm Atheros Bluetooth 4.0 (Currently not working)

WebCam: Lenovo EasyCamera

ThunderBolt Ports: N/A

# Current Status: Working & Not Working
1. Hardware Video Decoding : Fully Supported
2. Audio : Fully Working
3. WebCam: Fully Working
4. Card Reader : Not working
5. CD-Rom Reader&Writer : Fully Working
6. Ethernet : Possibly working? I've had mixed results.
7. Battery Percentage : Working
8. SSD/HDD : Fully Working
9. USB : Fully Working
10. Bluetooth & WiFi : WiFi working, Bluetooth not.
# Installation
1. From a real Mac or VM, Get the Install macOS Big Sur.app. Google it for details.
2. Put the app to /Applications
3. Insert a USB to Mac or VM and connect it. Take note of the USB name. 
4. execute "sudo /Applications/Install\ macOS\ Big\ Sur.app/Contents/Resources/createinstallmedia --volume /Volumes/(Your USB device name) (If you want to install macOS Big Sur)
5. Enter password of root (WARNING: THIS WILL WIPE DATA ON THE SELECTED DRIVE. BE EXTRA CAREFUL)
6. Wait until the making of bootable macOS Drive finishs 
7. Mount the USB's EFI using Terminal by typing "diskutil list" and find your USB named most likely "Install macOS Big Sur" above or below it there should be an EFI partition with the identifier something like "disk2s1" once you know the identifier type "sudo diskutil mount disk2s1" it will ask for your password and it should be mounted and copy the files from the zip file on the Releases page onto the EFI partition.
8. In the Laptop that you want to run Macintosh, enter Boot Menu and boot from USB
9. It may take a while to boot depending on what USB you have, just wait.
10. If the installer appears, then you're in the right place. Go to disk utility and Wipe the Disk as APFS. (WARNING: THIS WILL WIPE DATA ON THE SELECTED DRIVE. BE EXTRA CAREFUL)
11. Exit the disk utility and install macOS as instructed.
12. The computer will reboot 2~3 times. This is very normal and just select 'preboot' on every bootloader menu. 
13. If it was successful, the mac setup screen will appear. 
14. Finish Setup.
15. Go back into Terminal and mount the SSD/HDD EFI and your USB'S EFI
16. Copy the EFI files from the USB to your SSD/HDD
17. Unplug USB and reboot to test.
18. Done.


# If you encounter any problems during install, or there is something that doesn't work, please open a new issue with photos.
