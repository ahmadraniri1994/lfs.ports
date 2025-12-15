COMMENT = File type identification utility
VERSION = 5.46
REVISION = 0
CATEGORIES = tool
PKGNAME = file
HOMEPAGE = https://www.darwinsys.com/file/
ARCHIVE = file-5.46.tar.gz
LINK = https://astron.com/pub/file/file-5.46.tar.gz
SRCCD = archive
BUILD = make
BUILDDIR = file-5.46
AUTO_CONF = (cd ${BUILDDIR} && ./configure \
	--prefix=/usr \
	--sysconfdir=/etc \
	--libdir=/usr/lib \
	--datadir=/usr/share \
	--enable-static \
	--build=x86_64-pc-linux-musl)
MAKEOPT =

prepare:
	patch -p1 -d ${BUILDDIR} -i $(PWD)/file-5.46-pr-579-net147-fix-stack-overrun.patch

post_build:

post-install:

include /usr/share/mk/lfs.port.mk
