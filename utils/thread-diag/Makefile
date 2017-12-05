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
PKG_SOURCE_VERSION:=85486285068831d94ab37f8967b2c746563688d0
PKG_MIRROR_HASH:=bdafc3af08b507a61aec63b23c50b5c431243bae09f4a09caf7c574753e9a73e
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