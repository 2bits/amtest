infodir = ${prefix}/blah/blah/foobar
info_TEXINFOS = main.texi
## Sanity check.
installcheck-local:
	if test x$${infodir+set} != xset; then \
	  ls -l "$(DESTDIR)$(prefix)/blah/blah/foobar/" || exit 1; \
	  test -f "$(DESTDIR)$(prefix)/blah/blah/foobar/dir" || exit 1; \
	else \
	  ls -l "$(DESTDIR)$$infodir/" || exit 1; \
	  test -f "$(DESTDIR)$$infodir/dir" || exit 1; \
	fi
