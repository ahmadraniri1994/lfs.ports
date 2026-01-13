COMMENT = Official icon theme from the Numix project
VERSION = 25.12.15
REVISION = 0
CATEGORIES = icon
PKGNAME = numix
HOMEPAGE = https://numixproject.github.io/
ARCHIVE = numix-icon-theme-${VERSION}.tar.gz
LINK = https://github.com/numixproject/numix-icon-theme/archive/${VERSION}/numix-icon-theme-${VERSION}.tar.gz
SRCCD = archive
BUILD = custom
BUILDDIR = numix-icon-theme-${VERSION}

prepare:
	mkdir -p pkg/usr/share/icons

custom-build:
	mv ${BUILDDIR}/Numix pkg/usr/share/icons/
	mv ${BUILDDIR}/Numix-Light pkg/usr/share/icons/

post_build:

post-install:

include /usr/share/mk/lfs.port.mk
