dnl 
dnl  Copyright 2004,2005,2006,2007,2008 Free Software Foundation, Inc.
dnl  
dnl  This file is part of GNU Radio
dnl  
dnl  GNU Radio is free software; you can redistribute it and/or modify
dnl  it under the terms of the GNU General Public License as published by
dnl  the Free Software Foundation; either version 3, or (at your option)
dnl  any later version.
dnl  
dnl  GNU Radio is distributed in the hope that it will be useful,
dnl  but WITHOUT ANY WARRANTY; without even the implied warranty of
dnl  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
dnl  GNU General Public License for more details.
dnl  
dnl  You should have received a copy of the GNU General Public License
dnl  along with GNU Radio; see the file COPYING.  If not, write to
dnl  the Free Software Foundation, Inc., 51 Franklin Street,
dnl  Boston, MA 02110-1301, USA.
dnl 

AC_INIT(gsm-receiver,0.0.3)
AC_PREREQ(2.57)
AC_CONFIG_AUX_DIR([.])

m4_include([config/gr_standalone.m4])
GR_STANDALONE

dnl Check for libosmocore (gsmtap support)
PKG_CHECK_MODULES(LIBOSMOCORE, libosmocore >= 0.3.1)

AC_CONFIG_FILES([\
	  Makefile \
	  config/Makefile \
	  src/Makefile \
	  src/lib/Makefile \
	  src/lib/decoder/Makefile \
	  src/lib/decoder/openbtsstuff/Makefile \
	  src/python/Makefile \
	  gsm-receiver.pc   \
	])
dnl #	  doc/Makefile \
dnl #	  src/python/run_tests \

dnl run_tests is created from run_tests.in.  Make it executable.
#AC_CONFIG_COMMANDS([run_tests], [chmod +x src/python/run_tests])

AC_OUTPUT
