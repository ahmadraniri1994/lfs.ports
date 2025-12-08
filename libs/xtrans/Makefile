COMMENT = X transport library
VERSION = 1.6.0
REVISION = 0
CATEGORIES = libs
PKGNAME = xtrans
HOMEPAGE = https://xorg.freedesktop.org/
ARCHIVE = xtrans-${VERSION}.tar.xz
LINK = https://www.x.org/releases/individual/lib/${ARCHIVE}
SRCCD = archive
BUILD = make
BUILDDIR = xtrans-${VERSION}
AUTO_CONF = (cd ${BUILDDIR} && ./configure --prefix=/usr)  

prepare:

post_build:
	mkdir -p package/usr/lib
	mv package/usr/share/pkgconfig package/usr/lib

post-install:

include /usr/share/mk/lfs.port.mk
