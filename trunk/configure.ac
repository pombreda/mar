AC_INIT(mar/mar_main.c)

AM_INIT_AUTOMAKE(mar,0.9)
AM_CONFIG_HEADER(config.h)
dnl AM_MAINTAINER_MODE

dnl Checks for programs.
AC_PROG_CC
AC_PROG_INSTALL

if test "$GCC" = yes ; then
	CFLAGS="$CFLAGS -Wall"
fi

dnl AC_PROG_LIBTOOL
dnl AC_SUBST(LIBTOOL_DEPS)
AC_CHECK_LIB(bz2, BZ2_bzread, [], AC_MSG_ERROR([*** mar needs libbz2.a (from the bzip2 package)]))

dnl Checks for typedefs, structures, and compiler characteristics.
dnl AC_C_CONST
dnl AC_C_INLINE
dnl AC_HEADER_TIME

AC_OUTPUT(Makefile mar/Makefile)
