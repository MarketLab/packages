#
# Copyright (C) 2021 Marketlab Sp. z o.o.
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=croniter
PKG_VERSION:=1.0.15
PKG_RELEASE:=1

PYPI_NAME:=$(PKG_NAME)
PKG_HASH:=a70dfc9d52de9fc1a886128b9148c89dd9e76b67d55f46516ca94d2d73d58219

PKG_MAINTAINER:=Marcin Górski <m.gorski@marketlab.pl>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include ../pypi.mk
include $(INCLUDE_DIR)/package.mk
include ../python3-package.mk

define Package/python3-croniter
  SECTION:=lang
  CATEGORY:=Languages
  SUBMENU:=Python
  TITLE:= iteration for the datetime object with a cron like format
  URL:= https://github.com/kiorky/croniter
  DEPENDS:= +python3 +python3-dateutil
  VARIANT:=python3
endef

define Package/python3-croniter/description
  Croniter provides iteration for the datetime object with a cron like format.
endef

$(eval $(call Py3Package,python3-croniter))
$(eval $(call BuildPackage,python3-croniter))
