COMMENT = Unicode Character Database
VERSION = 17.0.0
REVISION = 0
CATEGORIES = db
PKGNAME = unicode_character_database
HOMEPAGE = https://www.unicode.org/
LINKS = https://www.unicode.org/Public/17.0.0/ucd/UCD.zip \
	https://www.unicode.org/Public/17.0.0/ucd/Unihan.zip \
	https://www.unicode.org/Public/17.0.0/emoji/emoji-sequences.txt \
	https://www.unicode.org/Public/17.0.0/emoji/emoji-zwj-sequences.txt \
	https://www.unicode.org/Public/17.0.0/emoji/emoji-test.txt
SRCCD = archive
BUILD = custom

prepare:
	for i in ${LINKS}; do wget -c $$i; done

custom-build:
	mkdir -p pkg/usr/share/unicode/emoji

	for i in UCD.zip Unihan.zip; do \
		bsdtar -C pkg/usr/share/unicode -x --no-same-owner \
		--no-same-permissions -f $$i; done

	for i in sequences test zwj-sequences; do \
		install -Dm644 emoji-$$i.txt pkg/usr/share/unicode/emoji/emoji-$$i.txt; \
		done

post_build:

post-install:

include /usr/share/mk/lfs.port.mk
