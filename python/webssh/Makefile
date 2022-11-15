#
# Copyright (C) 2022 TowerSoftware Ltd
#
# This is free software, licensed under the GNU General Public License v3.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-webssh
PKG_VERSION:=1.6.0
PKG_RELEASE:=1

PYPI_NAME:=webssh
PKG_HASH:=b7f60cc6f44741fb3fe227bcac90d9ab


PKG_LICENSE:=MIT
PKG_MAINTAINER:=DumTux <tekobase@outlook.com>

include ../pypi.mk
include $(INCLUDE_DIR)/package.mk
include ../python3-package.mk

define Package/python3-webssh
  SECTION:=lang-python
  CATEGORY:=TowerSoftware
  SUBMENU:=Python packages
  TITLE:=python3-webssh
  URL:=https://github.com/huashengdun/webssh
  DEPENDS:=+python3-light +python3-tornado +python3-paramiko
endef

define Package/python3-webssh/description
A simple web application to be used as an ssh client to connect to your ssh servers.
It is written in Python, base on tornado, paramiko and xterm.js.


endef

$(eval $(call Py3Package,python3-webssh))
$(eval $(call BuildPackage,python3-webssh))
