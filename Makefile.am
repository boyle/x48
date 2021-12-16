

AUTOMAKE_OPTIONS = dejagnu

SUBDIRS = src romdump

EXTRA_DIST=rpm/x48.spec README.md \
 debian/changelog debian/compat debian/control debian/copyright \
 debian/dirs debian/docs debian/menu debian/README.Debian debian/rules

X48 : src/X48.ad
	cp $< $@

appdefault_DATA = X48

README: README.md
	cp $< $@

DISTCHECK_CONFIGURE_FLAGS = --with-appdefaultdir='$${datadir}/X11/app-defaults'

