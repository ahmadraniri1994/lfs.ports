COMMENT = X11 Display Manager Control Protocol library
VERSION = 1.1.5
REVISION = 0
CATEGORIES = libs
PKGNAME = libXdmcp
HOMEPAGE = https://xorg.freedesktop.org/
ARCHIVE = libXdmcp-${VERSION}.tar.xz
LINK = https://www.x.org/releases/individual/lib/${ARCHIVE}
SRCCD = archive
BUILD = make
BUILDDIR = libXdmcp-${VERSION}
AUTO_CONF = (cd ${BUILDDIR} && ./configure --prefix=/usr --sysconfdir=/etc)

prepare:

post_build:

post-install:

include /usr/share/mk/lfs.port.mk
