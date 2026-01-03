COMMENT = Reference implementation of the Linux FUSE (Filesystem in Userspace) interface.
VERSION = 3.18.1
REVISION = 0
CATEGORIES = libs
PKGNAME = fuse3
HOMEPAGE = https://github.com/libfuse/libfuse/
ARCHIVE = fuse-3.18.1.tar.gz
LINK = https://github.com/libfuse/libfuse/releases/download/fuse-3.18.1/fuse-3.18.1.tar.gz
SRCCD = archive
BUILD = meson
BUILDDIR = fuse-3.18.1
BUILD_OPTION = -Dinitscriptdir="" \
	--default-library=both \
	--sbindir=/sbin

prepare:
	for i in patch/*; do patch -p1 -d ${BUILDDIR} -i $(PWD)/$$i; done

post_build:

post-install:

include /usr/share/mk/lfs.port.mk
