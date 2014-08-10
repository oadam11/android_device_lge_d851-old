#
# Copyright (C) 2014 The CyanogenMod Project
#
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
#      http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.
#

# CPU
TARGET_CPU_ABI := armeabi-v7a
TARGET_CPU_ABI2 := armeabi
TARGET_CPU_SMP := true
TARGET_ARCH := arm
TARGET_ARCH_VARIANT := armv7-a-neon
TARGET_CPU_VARIANT := krait
TARGET_USE_KRAIT_BIONIC_OPTIMIZATION := true
TARGET_USE_KRAIT_PLD_SET := true
TARGET_KRAIT_BIONIC_PLDOFFS := 10
TARGET_KRAIT_BIONIC_PLDTHRESH := 10
TARGET_KRAIT_BIONIC_BBTHRESH := 64
TARGET_KRAIT_BIONIC_PLDSIZE := 64
TARGET_GLOBAL_CFLAGS += -mfpu=neon -mfloat-abi=softfp
TARGET_GLOBAL_CPPFLAGS += -mfpu=neon -mfloat-abi=softfp

# Device
TARGET_NO_BOOTLOADER := true
TARGET_NO_RADIOIMAGE := true
TARGET_BOARD_PLATFORM := msm8974
TARGET_BOOTLOADER_BOARD_NAME := d851

# Kernel
BOARD_KERNEL_BASE := 0x00000000
BOARD_KERNEL_PAGESIZE := 2048
BOARD_KERNEL_CMDLINE := console=ttyHSL0,115200,n8 androidboot.hardware=d851 user_debug=31 msm_rtb.filter=0x0 LGD851 mdss_mdp.panel=1:dsi:0:qcom,mdss_dsi_lgit_sic_mipi0_video:1:qcom,mdss_dsi_lgit_sic_mipi1_video uart_console lge.rev=rev_10 lge.bootreason=0x0 lge.hreset=off gpt lge.kcal batt.soc=50 maxcpus=4 kswitch vmalloc=600m
BOARD_MKBOOTIMG_ARGS := --kernel_offset 0x0008000 --ramdisk_offset 0x2000000 --second_offset 0x0f00000 --tags_offset 0x0000100
BOARD_KERNEL_IMAGE_NAME := zImage-dtb
TARGET_KERNEL_SOURCE := kernel/lge/msm8974ac
TARGET_KERNEL_CONFIG := g3-tmo_us-perf_defconfig

# GPS
BOARD_VENDOR_QCOM_GPS_LOC_API_HARDWARE := $(TARGET_BOARD_PLATFORM)

# EGL
BOARD_EGL_CFG := device/lge/d851/egl.cfg
USE_OPENGL_RENDERER := true
TARGET_USES_ION := true

# Partitions
BOARD_BOOTIMAGE_PARTITION_SIZE := 14485760
BOARD_RECOVERYIMAGE_PARTITION_SIZE := 16485760
BOARD_SYSTEMIMAGE_PARTITION_SIZE := 1073741824
BOARD_USERDATAIMAGE_PARTITION_SIZE := 2147483648
BOARD_FLASH_BLOCK_SIZE := 131072 # (BOARD_KERNEL_PAGESIZE * 64)
BOARD_VOLD_EMMC_SHARES_DEV_MAJOR := true

# Recovery
RECOVERY_FSTAB_VERSION := 2
TARGET_USERIMAGES_USE_EXT4 := true
BOARD_HAS_NO_SELECT_BUTTON := true
TARGET_RECOVERY_PIXEL_FORMAT := "RGBX_8888"

-include vendor/lge/d851/BoardConfigVendor.mk
