COMMENT = X11 shared memory fences
VERSION = 1.3.3
REVISION = 0
CATEGORIES = libs
PKGNAME = libxshmfence
HOMEPAGE = https://www.x.org/
ARCHIVE = libxshmfence-${VERSION}.tar.xz
LINK = https://www.x.org/releases/individual/lib/${ARCHIVE}
SRCCD = archive
BUILD = make
BUILDDIR = libxshmfence-${VERSION}
AUTO_CONF = (cd ${BUILDDIR} && CFLAGS="-flto=auto" ./configure \
	--prefix=/usr \
	--disable-static \
	--enable-futex) 

prepare:

post_build:

post-install:

include /usr/share/mk/lfs.port.mk
