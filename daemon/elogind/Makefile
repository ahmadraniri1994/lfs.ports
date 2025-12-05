COMMENT = Standalone fork of systemd's elogind
VERSION = 255.22
REVISION = 0
CATEGORIES = daemon
PKGNAME = elogind
HOMEPAGE = https://github.com/elogind/elogind
ARCHIVE = elogind-V${VERSION}.tar.gz
LINK = ${HOMEPAGE}/archive/V${VERSION}/${ARCHIVE}
SRCCD = archive
BUILD = meson
BUILDDIR = elogind-${VERSION}
BUILD_OPTION = -Ddefault-kill-user-processes=false \
	-Dhalt-path=/sbin/halt \
	-Dman=disabled \
	-Dpolkit=enabled \
	-Dreboot-path=/sbin/reboot \
	-Dtests=false \
	-Dutmp=false \
	-Dpamconfdir=/etc/pam.d \
	-Dudevrulesdir=/lib/udev/rules.d \
	-Ddbuspolicydir=/etc/dbus-1/system.d \
	-Dcgroup-controller=elogind

prepare:
	for i in patch/*; do patch -p1 -d ${BUILDDIR} -i $(PWD)/$$i; done

post_build:
	ln -s libelogind.pc build/package/usr/lib/pkgconfig/libsystemd.pc
	ln -s libelogind.pc build/package/usr/lib/pkgconfig/libsystemd-logind.pc
	ln -s elogind build/package/usr/include/systemd 

	install -Dm644 ${BUILDDIR}/src/systemd/sd-id128.h build/package/usr/include
	install -Dm644 ${BUILDDIR}/src/systemd/_sd-common.h build/package/usr/include

post-install:

include /usr/share/mk/lfs.port.mk
