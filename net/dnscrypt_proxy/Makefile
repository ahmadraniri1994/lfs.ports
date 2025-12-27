COMMENT = A flexible DNS proxy, with support for encrypted DNS protocols.
VERSION = 2.1.15
REVISION = 0
CATEGORIES = net
PKGNAME = dnscrypt_proxy
HOMEPAGE = https://dnscrypt.info/
ARCHIVE = dnscrypt-proxy-linux_x86_64-2.1.15.tar.gz
LINK = https://github.com/DNSCrypt/dnscrypt-proxy/releases/download/2.1.15/dnscrypt-proxy-linux_x86_64-2.1.15.tar.gz
SRCCD = archive
BUILD = custom
BUILDDIR = linux-x86_64
PKGUSERS = dnscrypt
PKGGROUPS = dnscrypt

prepare:
	mkdir -p pkg/usr/bin
	install -dvm0755 -o ${PKGUSERS} -g ${PKGGROUPS} pkg/etc/dnscrypt-proxy \
		pkg/usr/share/dnscrypt-proxy \
		pkg/var/run/dnscrypt-proxy \
		pkg/var/cache/dnscrypt-proxy \
		pkg/var/log/dnscrypt-proxy

custom-build:
	install -D -m 0755 ${BUILDDIR}/dnscrypt-proxy \
		pkg/usr/bin/dnscrypt-proxy
	install -D -m 0644 ${BUILDDIR}/example-dnscrypt-proxy.toml \
		pkg/etc/dnscrypt-proxy/dnscrypt-proxy-example.toml

post_build:

post-install:

include /usr/share/mk/lfs.port.mk
