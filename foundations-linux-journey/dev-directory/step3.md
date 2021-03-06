Here are the most common device names that you will encounter: 

**SCSI Devices**

If you have any sort of mass storage on your machine, chances are it is using the SCSI (pronounced "scuzzy") protocol. SCSI stands for Small Computer System Interface, it is a protocol used for allow communication between disks, printers, scanners and other peripherals to your system. You may have heard of SCSI devices which aren't actually in use in modern systems, however our Linux systems correspond SCSI disks with hard disk drives in /dev. They are represented by a prefix of sd (SCSI disk):

Common SCSI device files:

* /dev/sda - First hard disk
* /dev/sdb - Second hard disk
* /dev/sda3 - Third partition on the first hard disk

**Pseudo Devices**

As we discussed earlier, pseudo devices aren't really physically connected to your system, most common pseudo devices are character devices: 

* /dev/zero - accepts and discards all input, produces a continuous stream of NULL (zero value) bytes
* /dev/null - accepts and discards all input, produces no output
* /dev/random - produces random numbers

**PATA Devices**

Sometimes in older systems you may see hard drives being referred to with an hd prefix: 

* /dev/hda - First hard disk
* /dev/hdd2 - Second partition on 4th hard disk 

## Exercise

Write to the pseudo devices and see what happens, be careful not to write your disks to those devices!

>>Q1: What would commonly be the device name for the first partition on the second SCSI disk?<<
=== sdb1
