#
# Copyright (C) 2010-2025 OpenWrt.org
# Copyright (C) 2025 lyin888 <lyin007@gmail.com>
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=Socat-expand
PKG_VERSION:=20250502
PKG_RELEASE:=1

include $(INCLUDE_DIR)/package.mk

define Package/Socat-expand
  TITLE:=Self-use expansion function.
  MAINTAINER:=Lyin888
  DEPENDS:=
  VARIANT:=
endef

define Package/Socat-expand/description
  Self-use expansion function.
endef

define Build/Compile
endef

define Package/Socat-expand/install
	$(INSTALL_DIR) $(1)/etc/init.d
	$(INSTALL_BIN) ./files/autocore $(1)/etc/init.d/autocore
	$(INSTALL_DIR) $(1)/etc
	$(INSTALL_DATA) ./files/socat $(1)/etc/socat
endef

$(eval $(call BuildPackage,Socat-expand))
