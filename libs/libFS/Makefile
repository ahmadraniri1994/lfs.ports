COMMENT = X font service client library
VERSION = 1.0.10
REVISION = 0
CATEGORIES = libs
PKGNAME = libFS
HOMEPAGE = https://www.x.org
ARCHIVE = libFS-1.0.10.tar.xz
LINK = https://www.x.org/releases/individual/lib/libFS-1.0.10.tar.xz
SRCCD = archive
BUILD = make
BUILDDIR = libFS-1.0.10
AUTO_CONF = (cd ${BUILDDIR} && ./configure \
	--prefix=/usr \
	--sysconfdir=/etc \
	--libdir=/usr/lib \
	--build=x86_64-pc-linux-musl)
MAKEOPT =

prepare:

post_build:

post-install:

include /usr/share/mk/lfs.port.mk
