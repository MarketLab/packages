#
# Copyright (C) 2021 Marketlab Sp. z o.o.
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=aiomqtt
PKG_VERSION:=0.1.3
PKG_RELEASE:=1

PYPI_NAME:=$(PKG_NAME)
PKG_HASH:=8c09676cbc1e682ea7b282fcd9bcae1b9630855dacc5180dbcacbee069b9576d

PKG_MAINTAINER:=Marcin Górski <m.gorski@marketlab.pl>
PKG_LICENSE:=epl-v10
PKG_LICENSE_FILES:=LICENSE

include ../pypi.mk
include $(INCLUDE_DIR)/package.mk
include ../python3-package.mk

define Package/python3-aiomqtt
  SECTION:=lang
  CATEGORY:=Languages
  SUBMENU:=Python
  TITLE:=Async paho-mqtt wrapper
  URL:=https://github.com/mossblaser/aiomqtt
  DEPENDS:= +python3 +python3-paho-mqtt
  VARIANT:=python3
endef

define Package/python3-aiomqtt/description
  This library implements a minimal Python 3 asyncio wrapper around the MQTT client in paho-mqtt
endef

$(eval $(call Py3Package,python3-aiomqtt))
$(eval $(call BuildPackage,python3-aiomqtt))
