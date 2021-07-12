#
# Copyright (C) 2021 Marketlab Sp. z o.o.
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=marshmallow-enum
PKG_VERSION:=1.5.1
PKG_RELEASE:=1

PYPI_NAME:=$(PKG_NAME)
PKG_HASH:=38e697e11f45a8e64b4a1e664000897c659b60aa57bfa18d44e226a9920b6e58

PKG_MAINTAINER:=Marcin Górski <m.gorski@marketlab.pl>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include ../pypi.mk
include $(INCLUDE_DIR)/package.mk
include ../python3-package.mk

define Package/python3-marshmallow-enum
  SECTION:=lang
  CATEGORY:=Languages
  SUBMENU:=Python
  TITLE:= Enum field for use with Marshmallow.
  URL:=https://pypi.org/project/marshmallow-enum/
  DEPENDS:= +python3
  VARIANT:=python3
endef

define Package/python3-marshmallow-enum/description
  Enum field for use with Marshmallow.
endef

$(eval $(call Py3Package,python3-marshmallow-enum))
$(eval $(call BuildPackage,python3-marshmallow-enum))
