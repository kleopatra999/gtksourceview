GENERATED_ITEMS =			\
	gtksourceview.vcxproj		\
	gtksourceview.vcxproj.filters	\
	gtksourceview-install.props	\
	math.h

MSVC10_HEADERS_LISTS =	\
	gtksourceview.vs10.headers

EXTRA_DIST =					\
	gtksourceview.sln			\
	gtksourceview-build-defines.props	\
	gtksourceview-gen-srcs.props		\
	gtksourceview-install.propsin		\
	gtksourceview-version-paths.props	\
	gtksourceview.vcxprojin			\
	gtksourceview.vcxproj.filtersin		\
	gtksourceview-install.vcxproj		\
	$(GENERATED_ITEMS)

gtksourceview-install.props: $(top_srcdir)/build/win32/vs10/gtksourceview-install.propsin $(MSVC10_HEADERS_LISTS)
	$(CPP) -P - <$(top_srcdir)/build/win32/vs10/gtksourceview-install.propsin >$@
	$(RM) $(MSVC10_HEADERS_LISTS)

math.h: $(top_srcdir)/build/win32/vs9/math.h
	cp $< $@

DISTCLEANFILES = $(GENERATED_ITEMS)

-include $(top_srcdir)/git.mk
