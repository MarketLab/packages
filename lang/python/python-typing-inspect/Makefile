#
# Copyright (C) 2021 Marketlab Sp. z o.o.
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=typing_inspect
PKG_VERSION:=0.7.1
PKG_RELEASE:=1

PYPI_NAME:=$(PKG_NAME)
PKG_HASH:=047d4097d9b17f46531bf6f014356111a1b6fb821a24fe7ac909853ca2a782aa

PKG_MAINTAINER:=Marcin Górski <m.gorski@marketlab.pl>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE


include ../pypi.mk
include $(INCLUDE_DIR)/package.mk
include ../python3-package.mk

define Package/python3-typing-inspect
  SECTION:=lang
  CATEGORY:=Languages
  SUBMENU:=Python
  TITLE:= Experimental API for runtime inspection of types defined in the standard typing module.
  URL:=https://pypi.org/project/typing-inspect/
  DEPENDS:= +python3 +python3-mypy-extensions +python3-typing-extensions
  VARIANT:=python3
endef

define Package/python3-typing-inspect/description
  Experimental API for runtime inspection of types defined in the standard typing module.
endef

$(eval $(call Py3Package,python3-typing-inspect))
$(eval $(call BuildPackage,python3-typing-inspect))
