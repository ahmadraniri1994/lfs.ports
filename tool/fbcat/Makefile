COMMENT = Framebuffer screenshot tool
VERSION = 0.5.2
REVISION = 0
CATEGORIES = tool
PKGNAME = fbcat
HOMEPAGE = https://github.com/jwilk/fbcat
ARCHIVE = fbcat-0.5.2.tar.gz
LINK = https://github.com/jwilk/fbcat/releases/download/0.5.2/fbcat-0.5.2.tar.gz
SRCCD = archive
BUILD = make
BUILDDIR = fbcat-0.5.2
MAKEOPT = LDFLAGS="-static"

prepare:
	sed -i -e '/PREFIX/s/=/?=/' -e '/DESTDIR/s/=/?=/' ${BUILDDIR}/Makefile

post_build:
	$(MAKE) -C ${BUILDDIR}/doc

post-install:

include /usr/share/mk/lfs.port.mk
