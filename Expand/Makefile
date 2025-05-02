#
# Copyright (C) 2010-2025 OpenWrt.org
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=Expand
PKG_VERSION:=20250502
PKG_RELEASE:=1

include $(INCLUDE_DIR)/package.mk

define Package/Expand
  TITLE:=
  MAINTAINER:=Lyin888
  DEPENDS:=
  VARIANT:=
endef

define Package/Expand/description
  Expand.
endef

define Build/Compile
endef

define Package/Expand/install
	$(INSTALL_DIR) $(1)/etc/init.d
	$(INSTALL_BIN) ./files/autocore $(1)/etc/init.d/autocore
	$(INSTALL_DIR) $(1)/etc
	$(INSTALL_DATA) ./files/socat $(1)/etc/socat
endef

$(eval $(call BuildPackage,Expand))
