#
# Description: Support install OpenWrt to EMMC, update the OpenWrt firmware or kernel, and backup/restore config.
# Borrow: luci-app-filetransfer, Vernesong, Flippy etc.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=luci-app-amlogic
PKG_LICENSE:=GPL-2.0 License
PKG_MAINTAINER:=ophub <https://github.com/ophub/luci-app-amlogic>
PKG_VERSION:=2.0
PKG_RELEASE:=3

LUCI_TITLE:= LuCI support for Amlogic S9xxx STB
LUCI_DEPENDS:=@(aarch64||arm) \
	    +luci-lib-fs \
	    +block-mount \
	    +blkid \
	    +parted \
	    +dosfstools \
	    +e2fsprogs \
	    +lsblk \
	    +pv \
	    +resize2fs \
	    +tune2fs \
	    +losetup \
	    +uuidgen
LUCI_PKGARCH:=all

include $(TOPDIR)/feeds/luci/luci.mk

# call BuildPackage - OpenWrt buildroot signature

