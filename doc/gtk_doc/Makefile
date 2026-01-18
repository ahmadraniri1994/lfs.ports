COMMENT = Documentation tool for public library API
VERSION = 1.35.0
REVISION = 0
CATEGORIES = doc
PKGNAME = gtk_doc
HOMEPAGE = https://wiki.gnome.org/DocumentationProject/GtkDoc
ARCHIVE = gtk-doc-1.35.0.tar.gz
LINK = https://gitlab.gnome.org/GNOME/gtk-doc/-/archive/1.35.0/gtk-doc-1.35.0.tar.gz
SRCCD = archive
BUILD = make
BUILDDIR = gtk-doc-1.35.0
AUTO_CONF = (cd ${BUILDDIR} && ./configure \
	--prefix=/usr \
	--sysconfdir=/etc \
	--libdir=/usr/lib \
	--with-highlight=highlight \
	--build=x86_64-pc-linux-musl)
MAKEOPT =

prepare:
	cd ${BUILDDIR} && ./autogen.sh

custom-build:

post_build:

post-install:

include /usr/share/mk/lfs.port.mk
