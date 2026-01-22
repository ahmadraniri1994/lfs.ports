COMMENT = GIO-style async APIs for most Flatpak portals
VERSION = 0.9.1
REVISION = 0
CATEGORIES = libs
PKGNAME = libportal
HOMEPAGE = https://github.com/flatpak/libportal
ARCHIVE = 0.9.1.tar.gz
LINK = https://github.com/flatpak/libportal/archive/refs/tags/0.9.1.tar.gz
SRCCD = archive
BUILD = meson
BUILDDIR = libportal-0.9.1
BUILD_OPTION = -Dbackend-gtk3=enabled \
	-Dbackend-gtk4=enabled \
	-Dbackend-qt5=disabled \
	-Ddocs=false

prepare:

post_build:

post-install:

include /usr/share/mk/lfs.port.mk
