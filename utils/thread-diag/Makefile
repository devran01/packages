#
# Copyright (c) 2017 ARM Limited.
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.

include $(TOPDIR)/rules.mk

PKG_NAME:=thread-diag
PKG_VERSION:=1.0.0
PKG_RELEASE:=1

PKG_BUILD_DIR:=$(BUILD_DIR)/thread-diag-$(PKG_VERSION)
PKG_SOURCE_PROTO:=git
PKG_SOURCE_URL:=https://github.com/devran01/thread-diagnostics.git
PKG_SOURCE_DATE:=2017-12-4
PKG_SOURCE_VERSION:=d17c0c94939f152d3898b7de8de33e334ba1f355
PKG_MIRROR_HASH:=1931e02cbac25a122c7e425b0b44526ce1697e022563399f8066a9abe446b86a
PKG_MAINTAINER:=Devaraj Ranganna <devaraj.ranganna@arm.com>

include $(INCLUDE_DIR)/package.mk

define Package/thread-diag
    SECTION:=utils
    CATEGORY:=Utilities
    TITLE:=Diagnostics information from the Thread network
endef

define Package/thread-diag/description
    Get the diagnostics information from the Thread network.
endef

define Package/thread-diag/install
	$(INSTALL_DIR) $(1)/usr/bin
	$(INSTALL_BIN) $(PKG_BUILD_DIR)/thread-diag $(1)/usr/bin/
endef

$(eval $(call BuildPackage,thread-diag))