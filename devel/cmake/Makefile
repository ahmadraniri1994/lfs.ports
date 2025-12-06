COMMENT =Cross-platform open-source make system.
VERSION =4.2.0
_V=4.2
REVISION =0
CATEGORIES =devel
PKGNAME =cmake
HOMEPAGE =https://www.cmake.org
ARCHIVE =cmake-${VERSION}.tar.gz
LINK =https://cmake.org/files/v${_V}/${ARCHIVE}
SRCCD =archive
BUILD =custom
BUILDDIR =cmake-${VERSION}

prepare:
	sed -i '/"lib64"/s/64//' ${BUILDDIR}/Modules/GNUInstallDirs.cmake

custom-build:
	cd ${BUILDDIR} && ./bootstrap \
		--prefix=/usr \
		--system-libuv \
		--system-expat \
		--system-zlib \
		--system-bzip2 \
		--system-libarchive \
		--no-system-jsoncpp \
		--no-system-curl \
		--no-system-cppdap \
		--no-system-nghttp2 \
		--generator=Ninja \
		--parallel=4
	ninja -C ${BUILDDIR} -j4
	DESTDIR="../pkg" ninja -C ${BUILDDIR} -j4 install

post_build:

post-install:

include /usr/share/mk/lfs.port.mk
