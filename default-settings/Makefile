#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=default-settings
PKG_RELEASE:=1
PKG_LICENSE:=GPL-3.0

include $(INCLUDE_DIR)/package.mk

define Package/default-settings
  SECTION:=luci
  CATEGORY:=LuCI
  TITLE:=LuCI support for Default Settings
  DEPENDS:=+luci +@LUCI_LANG_zh_Hans +luci-i18n-base-zh-cn
  PKGARCH:=all
endef

define Build/Compile
endef

define Package/default-settings/install
	$(INSTALL_DIR) $(1)/etc/uci-defaults
	$(INSTALL_BIN) ./files/default-settings $(1)/etc/uci-defaults/
endef

$(eval $(call BuildPackage,default-settings))
