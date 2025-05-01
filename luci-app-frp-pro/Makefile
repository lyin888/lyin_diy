# Copyright (C) 2025 lyin888 <lyin007@gmail.com>
#
# This is free software, licensed under the GNU General Public License v3.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=luci-app-frp-pro
PKG_VERSION:=20250501
PKG_RELEASE:=1

LUCI_TITLE:=LuCI support for frp
LUCI_DEPENDS:=+wget-ssl
LUCI_PKGARCH:=all

define Package/$(PKG_NAME)/conffiles
/etc/config/frp
endef

include $(TOPDIR)/feeds/luci/luci.mk

# call BuildPackage - OpenWrt buildroot signature
