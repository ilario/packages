# This is free software, licensed under the GNU General Public License v2.
# See /LICENSES for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=unique-append
PKG_VERSION:=0.1
PKG_RELEASE:=1
PKG_LICENSE:=GPL-2.0

include $(INCLUDE_DIR)/package.mk

define Package/$(PKG_NAME)
  SECTION:=utils
  CATEGORY:=Utilities
  TITLE:=Insert a line in file avoiding duplicates
  MAINTAINER:=Ilario Gelmetti <ilario@sindominio.net>
  PKGARCH:=all
endef

define Package/$(PKG_NAME)/description
  Takes a string and a file, appends the string to
  the file unless the string is already present there.
  Originally written by G10h4ck for being used in LibreMesh.
endef

define Build/Compile
endef

define Build/Configure
endef

define Package/$(PKG_NAME)/install
  $(INSTALL_DIR) $(1)/
  $(CP) ./files/* $(1)/
endef

$(eval $(call BuildPackage,$(PKG_NAME)))
