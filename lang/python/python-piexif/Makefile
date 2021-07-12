#
# Copyright (C) 2021 Marketlab Sp. z o.o.
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=piexif
PKG_VERSION:=1.1.3
PKG_RELEASE:=1

PYPI_NAME:=$(PKG_NAME)
PYPI_SOURCE_EXT:=zip
PKG_HASH:=83cb35c606bf3a1ea1a8f0a25cb42cf17e24353fd82e87ae3884e74a302a5f1b

PKG_MAINTAINER:=Marcin Górski <m.gorski@marketlab.pl>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include ../pypi.mk
include $(INCLUDE_DIR)/package.mk
include ../python3-package.mk

define Package/python3-piexif
  SECTION:=lang
  CATEGORY:=Languages
  SUBMENU:=Python
  TITLE:=Simplify exif manipulations with Python
  URL:=https://pypi.org/project/piexif/
  DEPENDS:= +python3
  VARIANT:=python3
endef

define Package/python3-piexif/description
  To simplify exif manipulations with Python. Writing, reading, and more...
endef

$(eval $(call Py3Package,python3-piexif))
$(eval $(call BuildPackage,python3-piexif))
