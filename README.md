# rpi4b-linux-ota-mender

This project demonstrates building and updating a custom Linux image for Raspberry Pi 4B using Yocto Project and Mender OTA framework.

## Overview

This project implements an OTA update mechanism for kernel images using the Yocto Project build system. It enables remote kernel updates without physical access to the device, ensuring seamless system maintenance and security patching.

## Features

- **OTA Kernel Updates**: Remote kernel image updates without physical intervention
- **Yocto Integration**: Built on the robust Yocto Project framework
- **Dual Boot Support**: A/B partition scheme for safe rollback capability
- **Update Verification**: Checksum validation and secure boot support
- **Rollback Mechanism**: Automatic fallback to previous kernel on boot failure

## Prerequisites

- **Host System Requirements**:
  - Ubuntu 20.04 LTS or later (or compatible Linux distribution)
  - Minimum 50GB free disk space
  - 8GB RAM (16GB recommended)
  - Python 3.6 or later

**Required Packages**:
```bash
  sudo apt-get install gawk wget git diffstat unzip texinfo gcc build-essential \
  chrpath socat cpio python3 python3-pip python3-pexpect xz-utils debianutils \
  iputils-ping python3-git python3-jinja2 libegl1-mesa libsdl1.2-dev pylint3 \
  xterm python3-subunit mesa-common-dev zstd liblz4-tool
```

**To build run** 

```
 ./build.sh
```


<p style="font-size: 50px;"><a href="https://drive.google.com/file/d/1VwIAHuHhnTEy4mI_JyF2RSm1vaQGG0CI/view?usp=sharing">Demo</a></p>