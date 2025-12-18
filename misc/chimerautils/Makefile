COMMENT = Chimera's core userland, based on FreeBSD
VERSION = 15.0.2
REVISION = 0
CATEGORIES = misc
PKGNAME = chimerautils
HOMEPAGE = https://github.com/chimera-linux/chimerautils
ARCHIVE = v15.0.2.tar.gz
LINK = https://github.com/chimera-linux/chimerautils/archive/refs/tags/v15.0.2.tar.gz
SRCCD = archive
BUILD = meson
BUILDDIR = chimerautils-15.0.2
BUILD_OPTION = --auto-features=disabled \
	--bindir=/usr/lib/${PKGNAME}/bin \
	--sbindir=/usr/lib/${PKGNAME}/sbin \
	--libexecdir=/usr/lib/${PKGNAME} \
	-Dinstall-lib=false \

prepare:

post_build:
	rm -r build/package/usr/share/man

post-install:

include /usr/share/mk/lfs.port.mk
