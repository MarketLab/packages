#
# Copyright (C) 2021 Marketlab Sp. z o.o.
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=typing_extensions
PKG_VERSION:=3.10.0.0
PKG_RELEASE:=1

PYPI_NAME:=$(PKG_NAME)
PKG_HASH:=50b6f157849174217d0656f99dc82fe932884fb250826c18350e159ec6cdf342

PKG_MAINTAINER:=Marcin Górski <m.gorski@marketlab.pl>
PKG_LICENSE:=PSF
PKG_LICENSE_FILES:=LICENSE

include ../pypi.mk
include $(INCLUDE_DIR)/package.mk
include ../python3-package.mk

define Package/python3-typing-extensions
  SECTION:=lang
  CATEGORY:=Languages
  SUBMENU:=Python
  TITLE:= Backported and Experimental Type Hints for Python
  URL:=https://pypi.org/project/typing-extensions/
  DEPENDS:= +python3
  VARIANT:=python3
endef

define Package/python3-typing-extensions/description
  Backported and Experimental Type Hints for Python
endef

$(eval $(call Py3Package,python3-typing-extensions))
$(eval $(call BuildPackage,python3-typing-extensions))
