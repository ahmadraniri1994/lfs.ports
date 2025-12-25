COMMENT = Small library with error codes.
VERSION = 1.57
REVISION = 0
CATEGORIES = libs
PKGNAME = libgpg_error
HOMEPAGE = https://www.gnupg.org
ARCHIVE = libgpg-error-1.57.tar.bz2
LINK = https://www.gnupg.org/ftp/gcrypt/libgpg-error/libgpg-error-1.57.tar.bz2
SRCCD = archive
BUILD = make
BUILDDIR = libgpg-error-1.57
AUTO_CONF = (cd ${BUILDDIR} && ./configure \
	--prefix=/usr \
	--sysconfdir=/etc \
	--libdir=/usr/lib \
	--enable-install-gpg-error-config \
	--build=x86_64-pc-linux-musl)
MAKEOPT =

prepare:

post_build:

post-install:

include /usr/share/mk/lfs.port.mk
