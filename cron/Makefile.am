MAINTAINERCLEANFILES = $(srcdir)/Makefile.in

CLEANFILES = refile-and-grok.sh

scriptdir = $(DSP_LIBEXEC_DIR)

dist_script_SCRIPTS = remove-xmls.pl

script_SCRIPTS = refile-and-grok.sh

EXTRA_DIST = refile-and-grok.sh.in

refile-and-grok.sh: refile-and-grok.sh.in Makefile
	sed -e 's,[@]DSC_DATA_DIR[@],$(DSC_DATA_DIR),g' \
        -e 's,[@]DSP_LIBEXEC_DIR[@],$(DSP_LIBEXEC_DIR),g' \
        < $(srcdir)/refile-and-grok.sh.in > refile-and-grok.sh
