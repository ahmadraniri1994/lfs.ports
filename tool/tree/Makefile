COMMENT = Tree is a recursive directory listing command.
VERSION = 2.2.1
REVISION = 0
CATEGORIES = tool
PKGNAME = tree
HOMEPAGE = https://oldmanprogrammer.net/source.php?dir=projects/tree
ARCHIVE = unix-tree-2.2.1.tar.gz
LINK = https://gitlab.com/OldManProgrammer/unix-tree/-/archive/2.2.1/unix-tree-2.2.1.tar.gz
SRCCD = archive
BUILD = make
BUILDDIR = unix-tree-2.2.1
MAKEOPT = MANDIR="pkg/usr/share/man"
override PREFIX = pkg/usr

prepare:
	mkdir -p pkg/usr/bin
	mkdir -p pkg/usr/share/man/man1

post_build:
	cp -r pkg/* package/
	mv package/tree package/usr/bin/
	install -m 644 ${BUILDDIR}/doc/tree.1 package/usr/share/man/man1/tree.1

post-install:

include /usr/share/mk/lfs.port.mk
