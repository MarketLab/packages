#
# Copyright (C) 2021 Marketlab Sp. z o.o.
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=tzlocal
PKG_VERSION:=2.1
PKG_RELEASE:=1

PYPI_NAME:=$(PKG_NAME)
PKG_HASH:=643c97c5294aedc737780a49d9df30889321cbe1204eac2c2ec6134035a92e44

PKG_MAINTAINER:=Marcin Górski <m.gorski@marketlab.pl>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include ../pypi.mk
include $(INCLUDE_DIR)/package.mk
include ../python3-package.mk

define Package/python3-tzlocal
  SECTION:=lang
  CATEGORY:=Languages
  SUBMENU:=Python
  TITLE:= Returns a tzinfo object with the local timezone information
  URL:= https://pypi.org/project/tzlocal/
  DEPENDS:= +python3
  VARIANT:=python3
endef

define Package/python3-tzlocal/description
  Returns a tzinfo object with the local timezone information.
endef

$(eval $(call Py3Package,python3-tzlocal))
$(eval $(call BuildPackage,python3-tzlocal))
