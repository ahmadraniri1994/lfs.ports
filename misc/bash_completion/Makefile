COMMENT = Command-line tab-completion for bash
VERSION = 2.17.0
REVISION = 0
CATEGORIES = misc
PKGNAME = bash_completion
HOMEPAGE = https://github.com/scop/bash-completion
ARCHIVE = bash-completion-2.17.0.tar.xz
LINK = https://github.com/scop/bash-completion/releases/download/2.17.0/bash-completion-2.17.0.tar.xz
SRCCD = archive
BUILD = make
BUILDDIR = bash-completion-2.17.0
AUTO_CONF = (cd ${BUILDDIR} && ./configure \
	--prefix=/usr \
	--sysconfdir=/etc \
	--libdir=/usr/lib \
	--build=x86_64-pc-linux-musl)
MAKEOPT =

prepare:
	autoreconf -fiv ${BUILDDIR}

post_build:

post-install:

include /usr/share/mk/lfs.port.mk
