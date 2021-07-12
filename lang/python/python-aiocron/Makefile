#
# Copyright (C) 2021 Marketlab Sp. z o.o.
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=aiocron
PKG_VERSION:=1.3
PKG_RELEASE:=1

PYPI_NAME:=$(PKG_NAME)
PKG_HASH:=7f7c343b5bb18695206714f038726e3795e6dfa69affcc25abe17838d51be69c

PKG_MAINTAINER:=Marcin Górski <m.gorski@marketlab.pl>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include ../pypi.mk
include $(INCLUDE_DIR)/package.mk
include ../python3-package.mk

define Package/python3-aiocron
  SECTION:=lang
  CATEGORY:=Languages
  SUBMENU:=Python
  TITLE:= cron jobs in python
  URL:=https://pypi.org/project/aiocron/
  DEPENDS:= +python3-croniter +python3-tzlocal +python3-pytz
  VARIANT:=python3
endef

define Package/python3-aiocron/description
  Cron jobs in python
endef

$(eval $(call Py3Package,python3-aiocron))
$(eval $(call BuildPackage,python3-aiocron))
