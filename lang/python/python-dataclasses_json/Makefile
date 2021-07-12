#
# Copyright (C) 2021 Marketlab Sp. z o.o.
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=dataclasses-json
PKG_VERSION:=0.5.4
PKG_RELEASE:=1

PYPI_NAME:=$(PKG_NAME)
PKG_HASH:=6c3976816fd3cdd8db3be2b516b64fc083acd46ac22c680d3dc24cb1d6ae3367

PKG_MAINTAINER:=Marcin Górski <m.gorski@marketlab.pl>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include ../pypi.mk
include $(INCLUDE_DIR)/package.mk
include ../python3-package.mk

define Package/python3-dataclasses-json
  SECTION:=lang
  CATEGORY:=Languages
  SUBMENU:=Python
  TITLE:= simple API for encoding and decoding dataclasses to and from JSON
  URL:=https://pypi.org/project/dataclasses-json/
  DEPENDS:= +python3 +python3-marshmallow +python3-marshmallow-enum +python3-typing-inspect +python3-stringcase
  VARIANT:=python3
endef

define Package/python3-dataclasses-json/description
  This library provides a simple API for encoding and decoding dataclasses to and from JSON.
endef

$(eval $(call Py3Package,python3-dataclasses-json))
$(eval $(call BuildPackage,python3-dataclasses-json))
