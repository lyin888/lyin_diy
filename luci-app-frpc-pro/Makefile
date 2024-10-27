# Copyright (C) 2024 Openwrt.org
#
# This is free software, licensed under the Apache License, Version 2.0 .
#

include $(TOPDIR)/rules.mk

PKG_NAME:=luci-app-frpc-pro
PKG_VERSION:=1.2
PKG_RELEASE:=1

LUCI_TITLE:=LuCI Support for frpc
LUCI_DEPENDS:=+wget
LUCI_PKGARCH:=all

define Package/$(PKG_NAME)/conffiles
/etc/frpc
endef

include $(TOPDIR)/feeds/luci/luci.mk

# call BuildPackage - OpenWrt buildroot signature