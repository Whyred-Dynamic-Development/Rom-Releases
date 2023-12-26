# Bouquet Flashing Guide

Note: This is a FBEv2 ROM with NO way to disable encryption (at least not for now)

## Clean Flash:
1. Download and flash the dynamic recovery provided
2. Download the ROM
3. Boot into recovery
4. Apply Update > Sideload ROM > adb sideload ROM.zip (change ROM.zip to actual rom filename)
5. Let it flash, if there are any errors its fine because your aren't yet on Dynamic partition, as long as the flash doesn't stop with an error it'll work
6. Format DATA
7. Reboot and enjoy!

## Issues

### PixelExperiene Only Issue:
If you get an error while flashing pixelexperience then please do the following:
1. Download this file or extract from zip: [super_empty.img](https://drive.google.com/file/d/1R2gQQN9E6qhClrWLg5APpg30G2oNMb1A/view?usp=drive_link)
2. `adb reboot fastboot` (important or just reboot to recovery and change to fastbootd mode)
3. `fastboot delete-logical-partition system_ext product system`
4. `fastboot wipe-super super_empty.img`
5. Flash rom normally

### Whyred Only issue:
If you are facing any type of issue with bootloops even after then formating data or if it fails to flash then please try this recovery
[https://yuki-kaze.my.id/0:/Miscellaneous/Recovery/derpfest13_qpr3_recovery.zip](https://yuki-kaze.my.id/0:/Miscellaneous/Recovery/derpfest13_qpr3_recovery.zip) and format data
