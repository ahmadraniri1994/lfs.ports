COMMENT = IPC library used by GnuPG.
VERSION = 3.0.2
REVISION = 0
CATEGORIES = libs
PKGNAME = libassuan
HOMEPAGE = https://www.gnupg.org
ARCHIVE = libassuan-3.0.2.tar.bz2
LINK = https://www.gnupg.org/ftp/gcrypt/libassuan/libassuan-3.0.2.tar.bz2
SRCCD = archive
BUILD = make
BUILDDIR = libassuan-3.0.2
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
