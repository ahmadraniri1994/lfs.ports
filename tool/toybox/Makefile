COMMENT = all-in-one Linux command line.
VERSION = 0.8.13
REVISION = 0
CATEGORIES = tool
PKGNAME = toybox
HOMEPAGE = http://landley.net/toybox/
ARCHIVE = 0.8.13.tar.gz
LINK = https://github.com/landley/toybox/archive/refs/tags/0.8.13.tar.gz
SRCCD = archive
BUILD = make
BUILDDIR = toybox-0.8.13
MAKEOPT = LDFLAGS="--static"
MKINST = no

prepare:
	$(MAKE) -C ${BUILDDIR} defconfig

post_build:
	install -D -m755 ${BUILDDIR}/toybox package/usr/bin/toybox

post-install:

include /usr/share/mk/lfs.port.mk
