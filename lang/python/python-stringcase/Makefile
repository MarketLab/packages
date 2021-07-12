#
# Copyright (C) 2021 Marketlab Sp. z o.o.
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=stringcase
PKG_VERSION:=1.2.0
PKG_RELEASE:=1

PYPI_NAME:=$(PKG_NAME)
PKG_HASH:=48a06980661908efe8d9d34eab2b6c13aefa2163b3ced26972902e3bdfd87008

PKG_MAINTAINER:=Marcin Górski <m.gorski@marketlab.pl>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

PYTHON3_PKG_SETUP_ARGS:=

include ../pypi.mk
include $(INCLUDE_DIR)/package.mk
include ../python3-package.mk

define Package/python3-stringcase
  SECTION:=lang
  CATEGORY:=Languages
  SUBMENU:=Python
  TITLE:= Convert string cases between camel case, pascal case, snake case etc
  URL:=https://pypi.org/project/stringcase/
  DEPENDS:= +python3
  VARIANT:=python3
endef

define Package/python3-stringcase/description
  Convert string cases between camel case, pascal case, snake case etc.
endef

$(eval $(call Py3Package,python3-stringcase))
$(eval $(call BuildPackage,python3-stringcase))
