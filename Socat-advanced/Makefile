# SPDX-License-Identifier: GPL-2.0-only
#
# Copyright (C) 2021 Lean <coolsnowwolf@gmail.com>
# Copyright (C) 2021-2024 ImmortalWrt.org
# Copyright (C) 2025 lyin888 <lyin007@gmail.com>

include $(TOPDIR)/rules.mk

PKG_NAME:=Socat-advanced
PKG_VERSION:=20250503
PKG_RELEASE:=2

PKG_LICENSE:=GPL-2.0-only

include $(INCLUDE_DIR)/package.mk

define Package/Socat-advanced
  SECTION:=luci
  CATEGORY:=LuCI
  TITLE:=LuCI support for Socat-advanced
  DEPENDS:=+luci
  PKGARCH:=all
endef

define Build/Compile
endef

define Package/Socat-advanced/install
	$(INSTALL_DIR) $(1)/etc/uci-defaults
	$(INSTALL_BIN) ./files/Socat-advanced $(1)/etc/uci-defaults/
	$(INSTALL_DIR) $(1)/etc
	$(INSTALL_DATA) ./files/socat $(1)/etc/socat
endef

$(eval $(call BuildPackage,Socat-advanced))
