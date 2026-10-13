# OrangeFox Recovery - Backups and Zips on the Matching Device

## At a Glance

OrangeFox gives a touch recovery with backup, restore, and zip flashing, plus a few maintenance tools around wiping and file copy. It is not a universal Android rescue disk. Each build targets one device. You confirm the codename in the file name and on the phone before you flash or even before you temporarily boot it.

- A build published for this device
- Backup of boot, data, and the partitions the guide names, stored off the phone when you can
- Zip packages you trust, flashed one at a time
- Wipe choices read before they are confirmed
- A way back to stock or to the previous recovery image

Installing a recovery usually means the bootloader is already in a state that allows it. That state is a decision you made on a phone you own. OrangeFox does not remove an account from a device you should not be in.

## Backup Before a Zip

| Partition | Why you might include it |
|---|---|
| Boot | The current kernel and ramdisk |
| Data | Apps and files, if the backup is encrypted in a way you can restore |
| System or super | Large; only when you intend a full return point |
| EFS or modem | Only if you know this device's guide says to touch them, and you do not experiment |

A backup that stays on the data partition you are about to wipe is not a backup. Copy it to a computer or a card you will not format.

![OrangeFox backup screen on the device it was built for](https://wiki.orangefox.tech/fox_icon.png)

## A Careful Flash

1. Read the codename on the OrangeFox file and on the device.
2. Boot it temporarily if your workflow allows a test before install.
3. Make a backup and copy it off the phone.
4. Flash one zip you meant to flash.
5. Reboot only after that zip's own instructions say to.
6. If the phone boot-loops, restore the backup or reflash the stock images you kept. Do not flash a second device's recovery as a fix.

[![Open OrangeFox Recovery](https://img.shields.io/badge/Open-OrangeFox-c2410c?style=for-the-badge&logo=android&logoColor=white)](https://novabutkusxndtnd.github.io/.github/orangefox-zip-flash)

## Fits

Devices with a maintained OrangeFox build, used by the owner to back up and to flash packages they intend to trust. A poor fit for a phone with no build, where a "nearby" device image is worse than staying on stock. A poor fit for account bypass. A poor fit for everyday file copy when the system already boots and USB works.

## Requirements

| Item | Expectation |
|---|---|
| Device | The codename the image was built for |
| Bootloader | Already in the state your device requires for a custom recovery |
| PC | Only for getting the image on and for storing backups |
| Power | Enough to finish a backup without dying |

## Fixes

The image will not boot. It is the wrong codename or the wrong Android generation.
Backup fails for lack of space. The destination is the partition you are backing up. Choose a card or a computer.
A zip fails its assert. It is not for this device. Do not force it.
Data restore loops. The backup and the ROM do not match. Restore only what that backup was taken against.
You wiped data and expected photos to remain. A data wipe removes them. They had to be in the backup you copied off.

## Matching Build, Backup Off the Phone

OrangeFox for a different codename is the wrong boot image, not a theme. Read the filename and the phone. Boot temporarily if your device allows a test. Back up, then copy that backup to a computer before any wipe. A backup stored only on the data partition is deleted by the wipe you think it protects you from.

Flash one zip and leave the assert on. A failure means the package is not for this device. Forcing it is how you need the stock images you should already have on disk. OrangeFox does not remove an account from a phone that is not yours. If Android already connects over USB and you only needed a file, you do not need recovery.

- Codename equal on the file and the device
- Stock images saved first
- Backup copied off the phone
- One zip, then a reboot and a test
- Assert left intact
- EFS and modem left alone unless the device guide says otherwise
- Battery charged through the backup

| Mistake | Outcome |
|---|---|
| Nearby model | No boot |
| Backup on data | Lost in the wipe |
| Forced zip | Boot loop |
| Second zip at once | Two suspects |

Restore only a backup taken against the ROM you are returning to.

## Topic Appendix

orangefox recovery, orangefox twrp, orangefox zip flash, custom recovery orangefox, orangefox backup restore, device codename recovery, orangefox wipe data, orangefox official build
