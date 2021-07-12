#
# Copyright (C) 2021 Marketlab Sp. z o.o.
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=marshmallow
PKG_VERSION:=3.12.2
PKG_RELEASE:=1

PYPI_NAME:=$(PKG_NAME)
PKG_HASH:=77368dfedad93c3a041cbbdbce0b33fac1d8608c9e2e2288408a43ce3493d2ff

PKG_MAINTAINER:=Marcin Górski <m.gorski@marketlab.pl>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include ../pypi.mk
include $(INCLUDE_DIR)/package.mk
include ../python3-package.mk

define Package/python3-marshmallow
  SECTION:=lang
  CATEGORY:=Languages
  SUBMENU:=Python
  TITLE:= library for converting complex datatypes
  URL:=https://pypi.org/project/marshmallow/
  DEPENDS:= +python3
  VARIANT:=python3
endef

define Package/python3-marshmallow/description
  An ORM/ODM/framework-agnostic library for converting complex datatypes, such as objects, to and from native Python datatypes
endef

$(eval $(call Py3Package,python3-marshmallow))
$(eval $(call BuildPackage,python3-marshmallow))
