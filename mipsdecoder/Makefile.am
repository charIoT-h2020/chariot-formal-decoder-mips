ACLOCAL_AMFLAGS=-I m4
AM_CPPFLAGS=-I$(top_srcdir) -I$(top_builddir)
LIBTOOL_DEPS = @LIBTOOL_DEPS@
libtool: $(LIBTOOL_DEPS)
	$(SHELL) ./config.status libtool

# Program
bin_PROGRAMS = unisim-mipsdecoder-1.0.0
unisim_mipsdecoder_1_0_0_SOURCES = main.cc 
unisim_mipsdecoder_1_0_0_LDADD = libunisim-mipsdecoder-1.0.0.la

# Dynamic Plugin
lib_LTLIBRARIES = libunisim-mipsdecoder-1.0.0.la
libunisim_mipsdecoder_1_0_0_la_SOURCES =  unisim/component/cxx/processor/mips/isa/disasm.cc unisim/util/forbint/debug/debug.cc unisim/util/forbint/contract/contract.cc unisim/util/symbolic/symbolic.cc architecture.cc instructions.cc formal_debug_bindings.cc mipssec_decoder.cc 
#libunisim_mipsdecoder_1_0_0_la_LDFLAGS = -shared -no-undefined
libunisim_mipsdecoder_1_0_0_la_LDFLAGS = -no-undefined

noinst_HEADERS =  unisim/component/cxx/processor/mips/isa/floating-point.isa unisim/component/cxx/processor/mips/isa/mips32r2.isa unisim/component/cxx/processor/mips/isa/mips64.isa unisim/component/cxx/processor/mips/isa/mipsel.isa unisim/component/cxx/processor/mips/isa/special.isa  unisim/component/cxx/processor/mips/isa/disasm.hh unisim/util/forbint/debug/debug.hh unisim/util/forbint/debug/instruction_callback.h unisim/util/inlining/inlining.hh unisim/util/arithmetic/arithmetic.hh unisim/util/endian/endian.hh unisim/util/forbint/contract/contract.hh unisim/util/forbint/contract/decsec_callback.h unisim/util/forbint/contract/domsec_callback.h unisim/util/forbint/contract/memsec_callback.h unisim/util/forbint/forbint.h unisim/util/identifier/identifier.hh unisim/util/symbolic/symbolic.hh    architecture.hh instructions.hh  
EXTRA_DIST =  m4/endian.m4 m4/ax_cflags_warn_all.m4 
sharedir = $(prefix)/share/unisim-mipsdecoder-1.0.0
dist_share_DATA = COPYING README INSTALL AUTHORS NEWS ChangeLog 
nobase_dist_share_DATA = 

BUILT_SOURCES=	$(top_builddir)/unisim/component/cxx/processor/mips/isa/mipsel.hh	$(top_builddir)/unisim/component/cxx/processor/mips/isa/mipsel.tcc
CLEANFILES=	$(top_builddir)/unisim/component/cxx/processor/mips/isa/mipsel.hh	$(top_builddir)/unisim/component/cxx/processor/mips/isa/mipsel.tcc
$(top_builddir)/unisim/component/cxx/processor/mips/isa/mipsel.tcc: $(top_builddir)/unisim/component/cxx/processor/mips/isa/mipsel.hh
$(top_builddir)/unisim/component/cxx/processor/mips/isa/mipsel.hh:  unisim/component/cxx/processor/mips/isa/floating-point.isa unisim/component/cxx/processor/mips/isa/mips32r2.isa unisim/component/cxx/processor/mips/isa/mips64.isa unisim/component/cxx/processor/mips/isa/mipsel.isa unisim/component/cxx/processor/mips/isa/special.isa
	$(GENISSLIB_PATH) -o $(top_builddir)/unisim/component/cxx/processor/mips/isa/mipsel -w 8 -I $(top_srcdir) $(top_srcdir)/unisim/component/cxx/processor/mips/isa/mipsel.isa
	 
