#
# Copyright (C) 2021 Marketlab Sp. z o.o.
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=mypy_extensions
PKG_VERSION:=0.4.3
PKG_RELEASE:=1

PYPI_NAME:=$(PKG_NAME)
PKG_HASH:=2d82818f5bb3e369420cb3c4060a7970edba416647068eb4c5343488a6c604a8

PKG_MAINTAINER:=Marcin Górski <m.gorski@marketlab.pl>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include ../pypi.mk
include $(INCLUDE_DIR)/package.mk
include ../python3-package.mk

define Package/python3-mypy-extensions
  SECTION:=lang
  CATEGORY:=Languages
  SUBMENU:=Python
  TITLE:= experimental extensions to the standard “typing” module 
  URL:=https://pypi.org/project/mypy-extensions/
  DEPENDS:= +python3
  VARIANT:=python3
endef

define Package/python3-mypy-extensions/description
  Module defines experimental extensions to the standard “typing” module that are supported by the mypy typechecker
endef

$(eval $(call Py3Package,python3-mypy-extensions))
$(eval $(call BuildPackage,python3-mypy-extensions))
