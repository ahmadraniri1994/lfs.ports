COMMENT = dwm-like bar for dwl
VERSION = 0.1.0
REVISION = 0
CATEGORIES = wayland
PKGNAME = somebar
HOMEPAGE = https://git.sr.ht/~raphi/somebar
ARCHIVE = ${VERSION}.tar.gz
LINK = https://git.sr.ht/~raphi/somebar/archive/${ARCHIVE}
SRCCD = git
BUILD = meson
BUILDDIR = somebar

prepare:
	cp ${BUILDDIR}/src/config.def.hpp ${BUILDDIR}/src/config.hpp
	${EDITOR} ${BUILDDIR}/src/config.hpp

post_build:

post-install:

include /usr/share/mk/lfs.port.mk
