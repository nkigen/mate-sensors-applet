# SMU-SYS plugin
plugindir = $(libdir)/mate-sensors-applet/plugins

AM_CPPFLAGS = -DMATELOCALEDIR=\""$(datadir)/locale/"\" \
	-DG_LOG_DOMAIN=\""Sensors Applet"\" \
	-DPIXMAPS_DIR=\""$(datadir)/pixmaps/$(PACKAGE)/"\" \
	-DDATADIR=\""$(datadir)"\" \
	-DLIBDIR=\""$(libdir)"\" \
        -DSYSCONFDIR=\""$(sysconfdir)"\" \
        -DPREFIX=\""$(prefix)"\" \
	-I$(top_srcdir) \
	$(GLIB_CFLAGS)

plugin_LTLIBRARIES = libsmu-sys.la

libsmu_sys_la_SOURCES = \
	smu-sys-plugin.h	\
	smu-sys-plugin.c

libsmu_sys_la_LDFLAGS = $(PLUGIN_LIBTOOL_FLAGS) $(GLIB_LIBS)
libsmu_sys_la_LIBADD = $(top_builddir)/lib/libmate-sensors-applet-plugin.la
