### Process this file with automake to produce Makefile.in

backgrounddir = $(datadir)/pixmaps/backgrounds/openindiana

background_DATA = \
	openindiana-default.jpg \
	blue-sky.jpg \
	calanques.jpg \
	cerulean.jpg \
	cubism.jpg \
	daisy.jpg \
	dandelion.jpg \
	dusk.jpg \
	purple-haze.jpg \
	sparkle.jpg \
	sunset.jpg \
	thunder.jpg \
	tuttifrutti.jpg \
	violet.jpg

metadata_in_files = openindiana-backgrounds.xml.in
metadatadir = $(datadir)/gnome-background-properties
metadata_DATA = $(metadata_in_files:.xml.in=.xml)
@INTLTOOL_XML_RULE@

noinst_DATA = openindiana-backgrounds.xml.in

CLEANFILES = \
	openindiana-backgrounds.xml \
	openindiana-backgrounds.xml.in

DISTCLEANFILES = $(CLEANFILES)

EXTRA_DIST = \
	$(background_DATA) \
	openindiana-backgrounds.xml.in.in

openindiana-backgrounds.xml.in: openindiana-backgrounds.xml.in.in Makefile
	$(SED) 's|%%DATADIR%%|$(datadir)|g' $< >$@

