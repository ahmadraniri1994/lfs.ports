COMMENT = A simple library for manipulating structured configuration files
VERSION = 1.8.2
REVISION = 0
CATEGORIES = libs
PKGNAME = libconfig
HOMEPAGE = https://www.hyperrealm.com/libconfig/libconfig.html
ARCHIVE = v1.8.2.tar.gz
LINK = https://github.com/hyperrealm/libconfig/archive/v1.8.2.tar.gz
SRCCD = archive
BUILD = make
BUILDDIR = libconfig-1.8.2
BUILD_OPTION =
AUTO_CONF = (cd ${BUILDDIR} && ./configure \
	--prefix=/usr \
	--sysconfdir=/etc \
	--libdir=/usr/lib \
	--build=x86_64-pc-linux-musl)
MAKEOPT =

prepare:
	autoreconf -fi ${BUILDDIR}

post_build:

post-install:

include /usr/share/mk/lfs.port.mk
