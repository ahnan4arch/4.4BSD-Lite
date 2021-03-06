# This file was generated automatically by configure.  Do not edit.
VPATH = .
links = 
host_alias = m68k-hp-bsd
host_cpu = m68k
host_vendor = hp
host_os = bsd
host_canonical = m68k-hp-bsd
target_alias = m68k-hp-bsd
target_cpu = m68k
target_vendor = hp
target_os = bsd
target_canonical = m68k-hp-bsd
host_makefile_frag = m68k-hp-bsd.mh
ALL=all.internal
# Makefile for GNU C++ class library (libg++)
#   Copyright (C) 1989, 1992 Free Software Foundation, Inc.
#   written by Doug Lea (dl@rocky.oswego.edu)

#This file is part of GNU libg++.

#GNU libg++ is free software; you can redistribute it and/or modify
#it under the terms of the GNU General Public License as published by
#the Free Software Foundation; either version 1, or (at your option)
#any later version.

#GNU libg++ is distributed in the hope that it will be useful,
#but WITHOUT ANY WARRANTY; without even the implied warranty of
#MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
#GNU General Public License for more details.

#You should have received a copy of the GNU General Public License
#along with GNU libg++; see the file COPYING.  If not, write to
#the Free Software Foundation, 675 Mass Ave, Cambridge, MA 02139, USA.

srcdir = .

prefix = /usr/local

exec_prefix = $(prefix)
bindir = $(exec_prefix)/bin
libdir = $(exec_prefix)/lib
tooldir = $(libdir)/m68k-hp-bsd

datadir = $(prefix)/lib
mandir = $(prefix)/man
man1dir = $(mandir)/man1
man2dir = $(mandir)/man2
man3dir = $(mandir)/man3
man4dir = $(mandir)/man4
man5dir = $(mandir)/man5
man6dir = $(mandir)/man6
man7dir = $(mandir)/man7
man8dir = $(mandir)/man8
man9dir = $(mandir)/man9
infodir = $(prefix)/info
includedir = $(prefix)/include
gxx_includedir = $(libdir)/g++-include
docdir = $(datadir)/doc

SHELL = /bin/sh

INSTALL = install -c
INSTALL_PROGRAM = $(INSTALL)
INSTALL_DATA = $(INSTALL)

AR = `if [ -f $${rootme}../binutils/ar ] ; \
	then echo $${rootme}../binutils/ar ; \
	else echo ar ; fi`

AR_FLAGS = qc
RANLIB = `if [ -f $${rootme}../binutils/ranlib ] ; \
	then echo $${rootme}../binutils/ranlib ; \
	else echo ranlib ; fi`
NM = `if [ -f $${rootme}../binutils/nm ] ; \
	then echo $${rootme}../binutils/nm ; \
	else echo nm ; fi`

MAKEINFO = `if [ -f $${rootme}../texinfo/C/makeinfo ] ; \
	then echo $${rootme}../texinfo/C/makeinfo ; \
	else echo makeinfo ; fi`

###**######################################################################
#
# Directories, paths, compilation flags and program names.
#
# If a macro needs to have a different value, then change it in the
# site/architecture specific makefile in the directory config !
#
# This file contains the documentation for the macros and possible values.
# Don't remove them even, if they are only comments !

LIBG++_DIST_VERSION = 2.3

# needed only for shared libraries on SunOS 4; the number must consist of
# <major number>.<minor number>
LIBG++_VERSION = 140.4

# ------- System-dependent defines

# g++ so specific flags
OSFLAG=

# ld or ld++ os specific libraries
#OSLIBS =

# Comment out the next line to disable incremental linking test
# (this test NOT included in 1.39.0, so don't re-enable) ??? H.S.
#TEST0=test0
#TEST0=

# targets for test-install
TEST_INSTALL 		= test-90S # test-90D
VERIFY_GXX_INSTALLATION = foo_main # dfoo_main


# You can override iostream (e.g. in a site- or host-Makefile fragment) to:
# iostream (Normal iostream library)
# old-stream (Old stream library; no longer supported)
# no-stream (If you don't want iostream to be prt of libg++)
IO_DIR = iostream
# You can override gperf to not build it at all
GPERF = gperf
SUBDIRS	=  genclass src $(IO_DIR) $(GPERF) utils tests etc test-install

ALL	=  verify-gxx-installation genclass src $(GPERF) $(UTILS)
CHECK	=  tests etc etc-tests
UTILS   =  # utils

#CC = `[ $(build_host) != $(host_alias) ] && host_prefix=$(host_alias)-;\
#	if [ -f $${rootme}..$(host_root)/$${host_prefix}gcc/gcc ] ; \
#	then echo $${rootme}..$(host_root)/$${host_prefix}gcc/gcc ; \
#	else echo $${host_prefix}gcc; fi`
CC = `if [ -f $${rootme}../gcc/gcc ] ; \
	then echo $${rootme}../gcc/gcc\\ -B$${rootme}../gcc/ ; \
	else echo cc ; fi`
CXX = `if [ -f $${rootme}../gcc/gcc ] ; \
v	then echo $${rootme}../gcc/gcc\\ -B$${rootme}../gcc/ ; \
	else echo gcc; fi`

CFLAGS = -g
CXXFLAGS = -g -O
XTRAFLAGS = `if [ -f $${rootme}../gcc/gcc ] ; \
	then echo -I$${rootme}../gcc/include ; \
	else echo ; fi`

INSTALLDIR = $(libdir)
TARGETLIB = libg++.a

# Objects from iostream to insert into into libg++.a.
IO_OBJECTS_TO_GET = *.o
# Similarly to insert objects for libiberty into libg++.a.
LIBIBERTY = libiberty
LIBIBERTY_OBJECTS_TO_GET = `cat needed-list` strerror.o strsignal.o

###**######################################################################
#
# now we can redefine all defined macros with configuration specific values !

#### host and target dependent Makefile fragments come in here.
INSTALL = install -c
INSTALL_DATA = install -c -m 644
# RANLIB = ranlib
# Use -nostdinc++ flag if your version of gcc understands it.
NOSTDINC = # -nostdinc++

# If the C include files are C++-ready (with extern "C"),
# define: HAVE_CPLUS_EXTERN = 1 and: WRAP_C_INCLUDES =
# If not, define HAVE_CPLUS_EXTERN = 0, and do not define WRAP_C_INCLUDES here.
HAVE_CPLUS_EXTERN = 0

# Flags to pass to gen-params when building _G_config.h.
# For example: G_CONFIG_ARGS = size_t="unsigned long"
G_CONFIG_ARGS =
##

FLAGS_TO_PASS= \
	"prefix=$(prefix)" \
	"exec_prefix=$(exec_prefix)" \
	"tooldir=$(tooldir)" \
	"AR=$(AR)" \
	"AR_FLAGS=$(AR_FLAGS)" \
	"CC=$(CC)" \
	"CXX=$(CXX)" \
	"CFLAGS=$(CFLAGS)" \
	"CXXFLAGS=$(CXXFLAGS)" \
	"RANLIB=$(RANLIB)" \
	"LOADLIBES=$(LOADLIBES)" \
	"LDFLAGS=$(LDFLAGS)" \
	"MAKEINFO=$(MAKEINFO)" \
	"XTRAFLAGS=$(XTRAFLAGS)" \
	"INSTALL=$(INSTALL)" \
	"INSTALL_DATA=$(INSTALL_DATA)" \
	"INSTALL_PROGRAM=$(INSTALL_PROGRAM)"

###**######################################################################
#
# compilation actions

.NOEXPORT:
.PHONY: all
all: $(TARGETLIB) rest-in-parallel

.PHONY: boltcc
boltcc:
	rootme=`pwd`/ ; export rootme ; $(MAKE) $(FLAGS_TO_PASS)

.PHONY: rest-in-parallel
rest-in-parallel: .stmp-genclass .stmp-tests .stmp-etc .stmp-gperf .stmp-utils

# We assume libiberty is made before .
$(TARGETLIB): _G_config.h in-src in-io stamp-$(TARGETLIB)

stamp-$(TARGETLIB): src/stamp $(IO_DIR)/stamp ../$(LIBIBERTY)/libiberty.a
#	-rm -f $(TARGETLIB)
	rootme=`pwd`/ ; export rootme ; cd src ; $(AR) $(AR_FLAGS) ../$(TARGETLIB) *.o
	rootme=`pwd`/; export rootme; cd $(IO_DIR); \
	   $(AR) $(AR_FLAGS) ../$(TARGETLIB) $(IO_OBJECTS_TO_GET)
	cd ../$(LIBIBERTY); \
	  $(AR) $(AR_FLAGS) ../libg++/$(TARGETLIB) $(LIBIBERTY_OBJECTS_TO_GET)
	$(RANLIB) $(TARGETLIB)
	@touch stamp-$(TARGETLIB)

in-src:
	@rootme=`pwd`/ ; export rootme ; cd src ; \
		$(MAKE) $(FLAGS_TO_PASS)

in-io:
	@rootme=`pwd`/ ; export rootme ; cd $(IO_DIR) ; \
		$(MAKE) $(FLAGS_TO_PASS) stamp

in-libiberty:
	@rootme=`pwd`/ ; export rootme ; cd ../$(LIBIBERTY) ; \
		$(MAKE) $(FLAGS_TO_PASS)

.PHONY: check
check:
	@rootme=`pwd`/ ; export rootme ; $(MAKE) subdir_do DO=check "DODIRS=$(SUBDIRS)" $(FLAGS_TO_PASS)

.stmp-genclass: $(TARGETLIB)
	@rootme=`pwd`/ ; export rootme ; cd genclass ; \
	  $(MAKE) $(FLAGS_TO_PASS)"gxx_includedir=$(gxx_includedir)"
	touch $@

.stmp-tests: $(TARGETLIB)
	@rootme=`pwd`/ ; export rootme ; cd tests ; \
	  $(MAKE) $(FLAGS_TO_PASS)
	touch $@

.stmp-etc: $(TARGETLIB)
	@rootme=`pwd`/ ; export rootme ; cd etc ; \
	  $(MAKE) $(FLAGS_TO_PASS)
	touch $@

.stmp-gperf: $(TARGETLIB)
	@if [ "x$(GPERF)" != "x" ]; then \
	   rootme=`pwd`/ ; export rootme ; cd $(GPERF) ; \
	      $(MAKE) $(FLAGS_TO_PASS); \
	 else true; fi
	touch $@

.stmp-utils: $(TARGETLIB)
	@if [ "x$(UTILS)" != "x" ]; then \
	   rootme=`pwd`/ ; export rootme ; cd $(UTILS) ; \
	     $(MAKE) $(FLAGS_TO_PASS); \
	 else true; fi
	touch $@

#
# Documentation 
#
.PHONY: info
info: libg++.info
	@rootme=`pwd`/ ; export rootme ; $(MAKE) subdir_do DO=info "DODIRS=$(SUBDIRS)"

libg++.info: $(srcdir)/libg++.texinfo
	$(MAKEINFO) -o libg++.info $(srcdir)/libg++.texinfo

.PHONY: install-info
install-info: libg++.info
	-parent=`echo $(infodir)|sed -e 's@/[^/]*$$@@'`; \
	if [ -d $$parent ] ; then true ; else mkdir $$parent ; fi
	-if [ -d $(infodir) ] ; then true ; else mkdir $(infodir) ; fi
	for i in *.info* ; do \
		$(INSTALL_DATA) $$i $(infodir)/$$i ; \
		chmod a-x $(infodir)/$$i ; \
	done
	@rootme=`pwd`/ ; export rootme ; $(MAKE) subdir_do DO=install-info "DODIRS=$(SUBDIRS)"

.PHONY: clean-info
clean-info:
	-rm -f *.info*
	@rootme=`pwd`/ ; export rootme ; $(MAKE) subdir_do DO=clean-info "DODIRS=$(SUBDIRS)"

# More doc (the paper kind)

libg++.dvi: $(srcdir)/libg++.texinfo
	TEXINPUTS=${TEXIDIR}:.:$$TEXINPUTS tex $(srcdir)/libg++.texinfo
	texindex libg++.??
	TEXINPUTS=${TEXIDIR}:.:$$TEXINPUTS tex $(srcdir)/libg++.texinfo

libg++.ps: libg++.dvi
	dvips libg++ -o
	
#
#
# Installation
#

.PHONY: install
# FIXME - libg++.a, _G_config.h, genclass are all target-dependent,
# and shoudl be installed in a target-dependent directory.
install: all
	-parent=`echo $(INSTALLDIR)|sed -e 's@/[^/]*$$@@'`; \
	if [ -d $$parent ] ; then true ; else mkdir $$parent ; fi
	-if [ -d $(INSTALLDIR) ] ; then true ; else mkdir $(INSTALLDIR) ; fi
	$(INSTALL_DATA) $(TARGETLIB) $(INSTALLDIR)/$(TARGETLIB)
	$(RANLIB) $(INSTALLDIR)/$(TARGETLIB)
	-if [ -d $(prefix) ] ; then true ; else mkdir $(prefix) ; fi
	-parent=`echo $(gxx_includedir)|sed -e 's@/[^/]*$$@@'`; \
	if [ -d $$parent ] ; then true ; else mkdir $$parent ; fi
	-if [ -d $(gxx_includedir) ] ; then true ; else mkdir $(gxx_includedir) ; fi
	-if [ -d $(gxx_includedir)/sys ] ; then true ; else mkdir $(gxx_includedir)/sys ; fi
	-if [ -d $(gxx_includedir)/gen ] ; then true ; else mkdir $(gxx_includedir)/gen ; fi
#	rm -f $(gxx_includedir)/_G_config.h ; \
	  $(INSTALL_DATA) _G_config.h $(gxx_includedir)/_G_config.h || exit 1;
	cd $(srcdir)/src; \
	for FILE in *.h gen/*.ccP gen/*.hP; do \
		rm -f $(gxx_includedir)/$$FILE ; \
		$(INSTALL_DATA) $$FILE $(gxx_includedir)/$$FILE || exit 1; \
		chmod a-x $(gxx_includedir)/$$FILE ; \
	done
	if [ "$(HAVE_CPLUS_EXTERN)" = "0" ]; then \
	    cd $(srcdir)/g++-include; \
	    for FILE in *.h sys/*.h; do \
		rm -f $(gxx_includedir)/$$FILE ; \
		$(INSTALL_DATA) $$FILE $(gxx_includedir)/$$FILE || exit 1; \
		chmod a-x $(gxx_includedir)/$$FILE ; \
	    done; \
	fi
	cd $(IO_DIR) ; $(MAKE) $(FLAGS_TO_PASS) "gxx_includedir=$(gxx_includedir)" install-include-files
	if [ "x$(GPERF)" != "x" ]; then \
	  cd gperf ; $(MAKE) $(FLAGS_TO_PASS) install; \
	else true; fi
	@for D in genclass $(UTILS) ; do \
		if [ -d $$D ] ; then \
			(cd $$D; $(MAKE) $(FLAGS_TO_PASS) "gxx_includedir=$(gxx_includedir)" install) ; \
		fi ; \
	done
	cd test-install; $(MAKE) $(TEST_INSTALL) \
	    CXX=$(bindir)/gcc COMPILE_FLAGS="" LIBS=-lg++

###**######################################################################
#
# Destructors
#

.PHONY: mostlyclean clean distclean realclean
.PHONY: do_mostlyclean do_clean do_distclean do_realclean

do_mostlyclean:
	rm -f *.o core \#* temp.c stamp-$(TARGETLIB)
do_clean: do_mostlyclean
#	rm -f  .stmp-* _G_config.h $(TARGETLIB)
	rm -f  .stmp-* $(TARGETLIB)
do_distclean: do_clean
#	rm -f *~ *.a config.status Makefile
	rm -f *~ *.a config.status

do_realclean: do_distclean
	rm -f libg++.info*

mostlyclean: do_mostlyclean
	@$(MAKE) subdir_do DO=mostlyclean "DODIRS=$(SUBDIRS)"
clean: do_clean
	@$(MAKE) subdir_do DO=clean "DODIRS=$(SUBDIRS)"
distclean:
	@$(MAKE) subdir_do DO=distclean "DODIRS=$(SUBDIRS)"
	@$(MAKE) do_distclean
realclean:
	@for D in $(SUBDIRS); do \
		echo "cd $$D; $(MAKE) realclean" ; \
		(cd $$D ; $(MAKE) realclean TRASH_FILES="$(TRASH_FILES)"); \
	done
	@$(MAKE) do_realclean

DIST_NAME = libg++-$(LIBG++_DIST_VERSION)

$(DIST_NAME).tar.Z: dist

# Making a dist:
# cvs rtag libgxx-x-yy libg++
# cvs co -r libgxx-x-yy libg++
# Sanitize
# TEMPORARILY: make dist-fix-Makefile -f Makefile.in
# cd {HERE}; make dist [-f Makefile.in]

# This is a temporay kludge until we can resolve an FSF/Cygnus inconsistency.
dist-fix-Makefile:
	sed -e '/gxx_includedir =/s|[(]tooldir|(libdir|' <Makefile.in >Makefile.foo
	mv Makefile.foo Makefile.in

dist: force
	cd ..; chmod og=u `find . -print`
	-mkdir ../$(DIST_NAME)
	rootdir=`(cd $(srcdir)/..; pwd)`; \
	cd ../$(DIST_NAME); \
	ln -s $${rootdir}/libg++ $${rootdir}/move-if-change \
	  $${rootdir}/Makefile.in $${rootdir}/configure \
	  $${rootdir}/config.sub $${rootdir}/configure.in \
	  $${rootdir}/README $${rootdir}/etc \
	  $${rootdir}/config $${rootdir}/libiberty .; \
	  mkdir include; cd include; \
            ln -s $${rootdir}/include/getopt.h $${rootdir}/include/obstack.h \
                $${rootdir}/include/ansidecl.h $${rootdir}/include/demangle.h .
	cd ..; tar -c -h -f - $(DIST_NAME) | compress -c >$(DIST_NAME).tar.Z
	rm -rf ../$(DIST_NAME)

force:
.PHONY: $(SUBDIRS) dist

subdir_do: force
	@for i in $(DODIRS); do \
		if [ -d ./$$i ] ; then \
			echo "cd $$i ; $(MAKE) $(DO) ::: $(FLAGS_TO_PASS)"; \
			if (cd $$i ; $(MAKE) $(DO) $(FLAGS_TO_PASS)) ; then true ; else exit 1 ; fi ; \
		else true ; fi ; \
	done

# with the gnu make, this is done automatically.

Makefile: $(srcdir)/Makefile.in $(host_makefile_frag) $(target_makefile_frag)
	rootme=`pwd`/ ; export rootme; \
	  CC="$(CC)"; export CC; CXX="$(CXX)"; export CXX; \
	  $(SHELL) ./config.status

#_G_config.h: ${srcdir}/utils/gen-params
#	rootme=`pwd`/ ; export rootme; \
#	CC="$(CC) $(XTRAFLAGS)"; export CC; \
#	CXX="$(CXX) $(XTRAFLAGS) $(NOSTDINC)"; export CXX; \
#	CONFIG_NM="$(NM)"; export CONFIG_NM; \
#	${srcdir}/utils/gen-params LIB_VERSION=$(LIBG++_DIST_VERSION) $(G_CONFIG_ARGS) >tmp-params.h
#	mv tmp-params.h _G_config.h

.NOEXPORT:
