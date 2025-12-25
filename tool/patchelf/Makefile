COMMENT = Small utility to modify the dynamic linker and RPATH of ELF executables
VERSION = 0.18.0
REVISION = 0
CATEGORIES = tool
PKGNAME = patchelf
HOMEPAGE = https://nixos.org/patchelf.html
ARCHIVE = patchelf-0.18.0.tar.gz
LINK = https://github.com/NixOS/patchelf/releases/download/0.18.0/patchelf-0.18.0.tar.gz
SRCCD = archive
BUILD = make
BUILDDIR = patchelf-0.18.0
AUTO_CONF = (cd ${BUILDDIR} && ./configure \
	--prefix=/usr \
	--sysconfdir=/etc \
	--libdir=/usr/lib \
	--build=x86_64-pc-linux-musl)
MAKEOPT =

prepare:
	for i in patch/*; do patch -p1 -d ${BUILDDIR} -i $(PWD)/$$i; done

post_build:

post-install:

include /usr/share/mk/lfs.port.mk
