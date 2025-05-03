#
# Copyright (C) 2010-2025 OpenWrt.org
# Copyright (C) 2025 lyin888 <lyin007@gmail.com>
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=Socat-Expand
PKG_VERSION:=20250503
PKG_RELEASE:=2

include $(INCLUDE_DIR)/package.mk

define Package/Socat-Expand
  TITLE:=Self-use expansion function.
  MAINTAINER:=lyin888
  DEPENDS:=
  VARIANT:=
endef

define Package/Socat-Expand/description
  Self-use expansion function.
endef

define Build/Compile
endef

define Package/Socat-Expand/install
	$(INSTALL_DIR) $(1)/etc/init.d
	$(INSTALL_BIN) ./files/Socat-Expand $(1)/etc/init.d/Socat-Expand
	$(INSTALL_DIR) $(1)/etc
	$(INSTALL_DATA) ./files/socat $(1)/etc/socat
endef

$(eval $(call BuildPackage,Socat-Expand))
