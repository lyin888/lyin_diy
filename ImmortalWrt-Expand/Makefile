# SPDX-License-Identifier: GPL-2.0-only
#
# Copyright (C) 2021 Lean <coolsnowwolf@gmail.com>
# Copyright (C) 2021-2024 ImmortalWrt.org
# Copyright (C) 2025 lyin888 <lyin007@gmail.com>

include $(TOPDIR)/rules.mk

PKG_NAME:=ImmortalWrt-Expand
PKG_VERSION:=20250502
PKG_RELEASE:=1

PKG_LICENSE:=GPL-2.0-only

include $(INCLUDE_DIR)/package.mk

define Package/ImmortalWrt-Expand
  SECTION:=luci
  CATEGORY:=LuCI
  TITLE:=LuCI support for ImmortalWrt-Expand
  DEPENDS:=+luci
  PKGARCH:=all
endef

define Build/Compile
endef

define Package/ImmortalWrt-Expand/install
	$(INSTALL_DIR) $(1)/etc/uci-defaults
	$(INSTALL_BIN) ./files/105-ImmortalWrt-Expand $(1)/etc/uci-defaults/
endef

$(eval $(call BuildPackage,ImmortalWrt-Expand))
