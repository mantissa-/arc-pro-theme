if !ENABLE_TRANSPARENCY
themedir        = $(datadir)/themes/Arc-Pro-solid
themedarkerdir  = $(datadir)/themes/Arc-Pro-Dusk-solid
themedarkdir    = $(datadir)/themes/Arc-Pro-Night-solid
else
themedir        = $(datadir)/themes/Arc-Pro
themedarkerdir  = $(datadir)/themes/Arc-Pro-Dusk
themedarkdir    = $(datadir)/themes/Arc-Pro-Night
endif

ithemedir       = $(DESTDIR)$(themedir)
ithemedarkerdir = $(DESTDIR)$(themedarkerdir)
ithemedarkdir   = $(DESTDIR)$(themedarkdir)


install-exec-hook:

install-data-local:

if ENABLE_PLANK

if ENABLE_LIGHT
	$(MKDIR_P) $(ithemedir)
	cp -R $(srcdir)/Arc-Plank/. $(ithemedir)/plank
endif # ENABLE_LIGHT

if ENABLE_DARKER
	$(MKDIR_P) $(ithemedarkerdir)
	cp -R $(srcdir)/Arc-Plank/. $(ithemedarkerdir)/plank
endif # ENABLE_DARKER

if ENABLE_DARK
	$(MKDIR_P) $(ithemedarkdir)
	cp -R $(srcdir)/Arc-Plank/. $(ithemedarkdir)/plank
endif # ENABLE_DARK
endif # ENABLE_PLANK


uninstall-local:


EXTRA_DIST = $(srcdir)/Arc-Plank
