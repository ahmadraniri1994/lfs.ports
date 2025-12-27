COMMENT = Desktop notification library
VERSION = 0.8.7
REVISION = 0
CATEGORIES = libs
PKGNAME = libnotify
HOMEPAGE = https://gitlab.gnome.org/GNOME/libnotify
ARCHIVE = libnotify-0.8.7.tar.xz
LINK = https://download.gnome.org/sources/libnotify/0.8/libnotify-0.8.7.tar.xz
SRCCD = archive
BUILD = meson
BUILDDIR = libnotify-0.8.7
BUILD_OPTION = -Dtests="false" \
	-Dintrospection=enabled \
	-Dgtk_doc=false \
	-Ddocbook_docs=disabled \
	-Dman=false

prepare:

post_build:

post-install:

include /usr/share/mk/lfs.port.mk
