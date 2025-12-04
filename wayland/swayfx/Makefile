COMMENT = SwayFX: Sway, but with eye candy!
VERSION = 0.5.3
REVISION = 0
CATEGORIES = wayland
PKGNAME = swayfx
HOMEPAGE = https://github.com/WillPower3309/swayfx
ARCHIVE = ${VERSION}.tar.gz
LINK = ${HOMEPAGE}/archive/refs/tags/${ARCHIVE}
SRCCD = archive
BUILD = meson
BUILDDIR = swayfx-${VERSION}
BUILD_OPTION = -Dsd-bus-provider=libelogind 

prepare:

post_build:
	install -Dm644 sway-portals.conf build/package/usr/share/xdg-desktop-portal/sway-portals.conf

post-install:

include /usr/share/mk/lfs.port.mk
