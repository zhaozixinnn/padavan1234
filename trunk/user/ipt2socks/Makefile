include $(ROOTDIR)/rules.mk

PKG_NAME:=ipt2socks
PKG_VERSION:=1.1.4

PKG_SOURCE:=$(PKG_NAME)-$(PKG_VERSION).tar.gz
PKG_SOURCE_URL:=https://codeload.github.com/zfl9/ipt2socks/tar.gz/v$(PKG_VERSION)?
PKG_HASH:=68dc76e63951d655c2fd9b420e175b5a75a50014d6db6e729398b41f2c988356

include $(INCLUDE_DIR)/package.mk

$(eval $(call BuildPackage,ipt2socks))

romfs:
	$(INSTALL_DIR) $(ROMFSDIR)/usr/bin
	$(INSTALL_BIN) $(PKG_BUILD_DIR)/ipt2socks $(ROMFSDIR)/usr/bin/ipt2socks
