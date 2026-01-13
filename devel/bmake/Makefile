COMMENT = Portable version of the NetBSD make build tool
VERSION = 20251111
REVISION = 0
CATEGORIES = devel
PKGNAME = bmake
HOMEPAGE = https://www.crufty.net/help/sjg/bmake.html
ARCHIVE = bmake-20251111.tar.gz
LINK = https://www.crufty.net/ftp/pub/sjg/bmake-20251111.tar.gz
SRCCD = archive
BUILD = custom
BUILDDIR = bmake

prepare:

custom-build:
	cd ${BUILDDIR} && sh ./boot-strap \
		--with-default-sys-path=/usr/share/mk op=build
	cd ${BUILDDIR} && sh ./boot-strap \
		--prefix=/usr --with-mksrc=/usr/share/mk \
		--install-destdir="$(PWD)/pkg" op=install

post_build:
	rm -rf pkg/usr/share/man/cat1

	install -Dm644 ${BUILDDIR}/bmake.1 \
		pkg/usr/share/man/man1/bmake.1

	install -Dm644 ${BUILDDIR}/{README,ChangeLog} \
		-t pkg/usr/share/doc/bmake/

post-install:

include /usr/share/mk/lfs.port.mk
