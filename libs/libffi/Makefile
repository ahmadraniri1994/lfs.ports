COMMENT = portable, high level programming interface to various calling conventions.
VERSION = 3.5.2
REVISION = 0
CATEGORIES = libs
PKGNAME = libffi
HOMEPAGE = https://sourceware.org/libffi/
ARCHIVE = libffi-3.5.2.tar.gz
LINK = https://github.com/libffi/libffi/releases/download/v3.5.2/libffi-3.5.2.tar.gz
SRCCD = archive
BUILD = make
BUILDDIR = libffi-3.5.2
AUTO_CONF = (cd ${BUILDDIR} && ./configure \
	--prefix=/usr \
	--sysconfdir=/etc \
	--libdir=/usr/lib \
	--build=x86_64-pc-linux-musl \
	--enable-static \
	--with-gcc-arch=native \
	--enable-pax_emutramp \
	--enable-portable-binary \
	--disable-exec-static-tramp)
MAKEOPT =

prepare:

post_build:

post-install:

include /usr/share/mk/lfs.port.mk
