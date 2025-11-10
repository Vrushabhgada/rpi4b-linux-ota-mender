# ECEN 5713 AESD Fall 2025 Final Project

## Project Overview

[Project Overview Link](https://github.com/VrushabhGadaCU/final-project-assignment-OTA-SecureBoot/wiki)

## Project Schedule

[Project Schedule Link](https://github.com/users/VrushabhGadaCU/projects/2/views/1)


# Yocto Image for RPi 4 B

To Compile the image run the following command

```
./build.sh
```


Once you are done with building the image you run following command to flash the image 

```
cd build/tmp/deploy/images/raspberrypi4-64/
bunzip2 -dkf core-image-minimal-raspberrypi4-64.wic.bz2
sudo dd if=core-image-minimal-raspberrypi4-64.wic of=/dev/sdb bs=4M status=progress conv=fsync
sync
sudo eject /dev/sdb
```