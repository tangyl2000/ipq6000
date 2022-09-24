include $(TOPDIR)/rules.mk

ARCH:=aarch64
BOARD:=ipq60xx
BOARDNAME:=Qualcomm Atheros IPQ60xx
FEATURES:=squashfs fpu ramdisk nand
MAINTAINER:=John Crispin <john@phrozen.org>
CPU_TYPE:=cortex-a53
SUBTARGETS:=generic

KERNEL_PATCHVER:=4.4

KERNELNAME:=Image dtbs

include $(INCLUDE_DIR)/target.mk
DEFAULT_PACKAGES += \
	kmod-leds-gpio kmod-gpio-button-hotplug swconfig \
	kmod-qca-nss-dp kmod-qca-nss-drv kmod-qca-ssdk \
	kmod-qca-nss-drv-pppoe kmod-qca-nss-ecm \
	uboot-envtools qca-ssdk-shell nss-firmware-ipq6018

$(eval $(call BuildTarget))
