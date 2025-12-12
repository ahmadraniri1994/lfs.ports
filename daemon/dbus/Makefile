COMMENT = Freedesktop.org message bus system
VERSION = 1.16.2
REVISION = 1
CATEGORIES = daemon
PKGNAME = dbus
HOMEPAGE = https://www.freedesktop.org/Software/dbus
ARCHIVE = dbus-1.16.2.tar.xz
LINK = https://dbus.freedesktop.org/releases/dbus/dbus-1.16.2.tar.xz
SRCCD = archive
BUILD = meson
BUILDDIR = dbus-1.16.2
BUILD_OPTION =

prepare:

post_build:
	chmod 4750 build/package/usr/libexec/dbus-daemon-launch-helper
	chown -h root:messagebus build/package/usr/libexec/dbus-daemon-launch-helper

post-install:
	/usr/bin/dbus-uuidgen --ensure
	chmod 4750 /usr/libexec/dbus-daemon-launch-helper
	chown -h root:messagebus /usr/libexec/dbus-daemon-launch-helper

include /usr/share/mk/lfs.port.mk
