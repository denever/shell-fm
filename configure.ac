#                                               -*- Autoconf -*-
# Process this file with autoconf to produce a configure script.

AC_PREREQ(2.59)
AC_INIT([shell-fm], [0.6.0], [Jonas Kramer])
AC_CONFIG_AUX_DIR(config)
AM_CONFIG_HEADER(config.h)
AM_INIT_AUTOMAKE([dist-bzip2])

# Checks for programs.
AC_PROG_CXX
AC_PROG_INSTALL
#AC_PROG_RANLIB

# Checks for header files.
AC_HEADER_STDC	    

# Checks for libraries: libao, libmad
PKG_CHECK_MODULES([AO], [ao >= 0.8])
PKG_CHECK_EXISTS([AO], [ao >= 0.8], AC_DEFINE([LIBAO], [1], [Have libao]) )
PKG_CHECK_MODULES([MAD], [mad >= 0.14])
PKG_CHECK_EXISTS([MAD], [mad >= 0.8], AC_DEFINE([LIBMAD], [1], [Have libmad]))

# Checks for typedefs, structures, and compiler characteristics.
#AC_HEADER_STDBOOL
#AC_C_CONST
#AC_C_INLINE

# Checks for library functions.
#AC_PROG_GCC_TRADITIONAL
#AC_CHECK_FUNCS([floor])

AC_SUBST(AO_LIBS)
AC_SUBST(MAD_LIBS)

AC_SUBST(AO_CFLAGS)
AC_SUBST(MAD_CFLAGS)

AC_CONFIG_FILES([Makefile
		 include/Makefile
                 src/Makefile])
AC_OUTPUT
