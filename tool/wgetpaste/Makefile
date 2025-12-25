COMMENT = Command-line interface to various pastebins
VERSION = 2.34
REVISION = 0
CATEGORIES = tool
PKGNAME = wgetpaste
HOMEPAGE = http://wgetpaste.zlin.dk/
ARCHIVE = 2.34.tar.gz
LINK = https://github.com/zlin/wgetpaste/archive/2.34.tar.gz
SRCCD = archive
BUILD = custom
BUILDDIR = wgetpaste-2.34

prepare:

custom-build:
	install -Dm755 ${BUILDDIR}/wgetpaste pkg/usr/bin/wgetpaste 

post_build:

post-install:

include /usr/share/mk/lfs.port.mk
