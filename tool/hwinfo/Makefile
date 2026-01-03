COMMENT = Hardware information tool
VERSION = 25.0
REVISION = 0
CATEGORIES = tool
PKGNAME = hwinfo
HOMEPAGE = https://github.com/openSUSE/hwinfo
ARCHIVE = 25.0.tar.gz
LINK = https://github.com/openSUSE/hwinfo/archive/25.0.tar.gz
SRCCD = archive
BUILD = make
BUILDDIR = hwinfo-25.0
MAKEOPT = HWINFO_VERSION=${VERSION} LIBDIR=/usr/lib
MAKEFLAGS += -j1

prepare:
	echo 'touch changelog' > ${BUILDDIR}/git2log
	sed -i '/linux\/fs.h/d' ${BUILDDIR}/src/hd/hd.c

post_build:
	mv package/usr/sbin package/usr/bin

post-install:

include /usr/share/mk/lfs.port.mk
