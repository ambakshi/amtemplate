AC_INIT([amtemplate],[1.0],[abakshi@gmail.com])
AC_CONFIG_MACRO_DIR([m4])
AC_CONFIG_AUX_DIR([.build-aux])
AM_INIT_AUTOMAKE([foreign -Wall -Werror])
LT_INIT
AC_PROG_CC

#
AC_CHECK_HEADER([$HOME/something/x.h], [use_something=yes])
AM_CONDITIONAL([WANT_SOMETHING], [test "$use_something" = yes])

AX_FUNC_MKDIR_ONE_ARG

AC_CHECK_LIB([efence], [malloc], [EFENCELIB=-lefence])
AC_SUBST([EFENCELIB])
AC_CONFIG_HEADERS([include/config.h])
AC_CONFIG_FILES([Makefile src/Makefile src/something/Makefile])
AC_OUTPUT
