# TWRP samsung_a52sxq

Partially working TWRP custom recovery for Samsung Galaxy A52s 5G

***What doesn't work:***

- Touchscreen doesn't work
- Some partitions don't mount

If you want to get around the not working touchscreen problem connect a usb mouse via OTG cable to the phone.


**How to flash using ODIN**

Your bootloader should be unlocked!

1. Download the recovery image from this github repo.

2. Install 7-Zip: https://www.7-zip.org/download.html
3. Right click on recovery.img > 7-Zip > Add to archive. (Archive format .tar)

4. Download ODIN: https://www.odinflash.com/

5. Put the recovery.tar file to the AP slot in ODIN. 

6. While your phone is powered off, hold both volume up and volume down buttons and then connect your phone to the computer using usb cable. Once there is a prompt on a phone, click volume up button, your phone should be detected in ODIN. 

7. Click Start on odin to start flashing.

**How to unpack/repack the image**

`git clone https://github.com/arminask/TWRP-samsung_a52sxq.git`

`cd TWRP-samsung_a52sxq`

**To unpack the image**

`./unpackimg.sh`

2 folders should appear: *ramdisk* and *split_img*

**To repack the image**

`./repackimg.sh`

An image should be generated with a name *image_new.img*
