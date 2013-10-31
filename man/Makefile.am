#

dist_man_MANS = varnish-vmod-var.3
MAINTAINERCLEANFILES = $(dist_man_MANS)
EXTRA_DIST = varnish-vmod-var.rst

varnish-vmod-var.3: varnish-vmod-var.rst
if HAVE_RST2MAN
	${RST2MAN} varnish-vmod-var.rst $@
else
	@echo "========================================"
	@echo "You need rst2man installed to make dist"
	@echo "========================================"
	@false
endif
