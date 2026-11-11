**********************************************************************
***                  THIS IS NOT A FLASHABLE PACKAGE               ***
***                                                                ***
***  DO NOT FASTBOOT FLASH THIS PACKAGE OR ATTEMPT TO FLASH IT     ***
***  USING ANY OTHER AUTOMATED OR WHOLE-PACKAGE FLASHING METHOD.   ***
**********************************************************************

onn. 7 Core Stock Partition Dump
================================

Device:
  onn. 7 Core
  Model: 36020962
  Codename: onn7core

Software:
  Android 16
  Build: BP2A.250605.031.A3
  Incremental / build date identifier: 20260623

About this package
------------------
This package contains stock partition images dumped from an onn. 7 Core
(model 36020962) running the build listed above.

This is NOT an official factory firmware package from onn. or Walmart.
It is a device-derived partition dump intended for recovery, research,
development, and preservation.

This is NOT a flash-all package.

Package layout
--------------
partitions/
  boot_b.img
  dtbo_b.img
  init_boot_b.img
  super_stock.img
  vbmeta_b.img
  vbmeta_system_b.img
  vbmeta_vendor_b.img
  vendor_boot_b.img

advanced/
  boot0.bin
  boot_para.img
  lk_b.img
  preloader_b.bin

SHA256SUMS.txt
  SHA-256 hashes for all included images.

IMPORTANT
---------
The files in the "advanced" directory are low-level boot / platform images.

DO NOT blindly flash these files.

In particular, preloader and boot-region images can potentially render a
MediaTek device unbootable or require specialized recovery methods if they
are written incorrectly.

Only flash individual partitions if you fully understand what you are doing
and have verified:
  - Exact device model
  - Exact firmware/build compatibility
  - Correct partition name
  - Correct active slot / flashing method

A/B / dynamic partitions
------------------------
This device uses A/B partitioning and dynamic partitions.

The included boot-chain images were dumped from slot B.

super_stock.img contains the dynamic-partition container as dumped from the
device. Individual logical partitions extracted during analysis are not
included because the original super image is preserved here instead.

Integrity
---------
Verify files against SHA256SUMS.txt before using them.

Disclaimer
----------
Use at your own risk.

These files are provided for development and recovery purposes. Flashing
incorrect images or flashing them to a different device/build may cause
boot failure or device damage.

Author / source
---------------
Dump preserved and shared by AndroidMike1971
