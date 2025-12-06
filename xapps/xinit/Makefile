COMMENT = X Window System initializer.
VERSION = 1.4.4
REVISION = 0
CATEGORIES = xapps
PKGNAME = xinit
HOMEPAGE = https://www.x.org
ARCHIVE = xinit-${VERSION}.tar.gz
LINK = https://www.x.org/releases/individual/app/${ARCHIVE}
SRCCD = archive
BUILD = make
BUILDDIR = xinit-${VERSION}
AUTO_CONF = (cd ${BUILDDIR} && ./configure --prefix=/usr \
	--with-xinitdir=/etc/X11/xinit)

prepare:

post_build:

post-install:

include /usr/share/mk/lfs.port.mk
