#
# Copyright (C) 2025 Pascal Beleiu <pascal@beleiu.de>
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=zyxel-nwa210ax-bootconfig
PKG_RELEASE:=1

include $(INCLUDE_DIR)/package.mk

define Package/zyxel-nwa210ax-bootconfig
	SECTION:=utils
	CATEGORY:=Base system
	TITLE:=Utility that can change bootconfig settings for Zyxel NWA210AX
	MAINTAINER:=Pascal Beleiu <pascal@beleiu.de>
endef

define Package/zyxel-nwa210ax-bootconfig/description
	This package contains an utility that allows changing bootconfig settings for Zyxel NWA210AX.
endef

define Build/Prepare
	$(CP) src/zyxel-nwa210ax-bootconfig $(PKG_BUILD_DIR)/
endef

define Build/Compile
	true
endef

define Package/zyxel-nwa210ax-bootconfig/install
	$(INSTALL_DIR) $(1)/usr/bin
	$(INSTALL_BIN) $(PKG_BUILD_DIR)/zyxel-nwa210ax-bootconfig $(1)/usr/bin/
endef

$(eval $(call BuildPackage,zyxel-nwa210ax-bootconfig))
