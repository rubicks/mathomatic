#                                               -*- Autoconf -*-
# Process this file with autoconf to produce a configure script.

AC_PREREQ([2.69])
AC_INIT([mathomatic], [16.0.5], [rubicks00@gmail.com])
AC_LANG_PUSH([C])
AM_INIT_AUTOMAKE
AC_CONFIG_SRCDIR([diff.c])
AC_CONFIG_HEADERS([config.h])

# Checks for programs.
AC_PROG_CXX
AC_PROG_AWK
AC_PROG_CC
AC_PROG_RANLIB
AC_PROG_INSTALL
AC_PROG_LN_S

# Checks for libraries.
# FIXME: Replace `main' with a function in `-lm':
AC_CHECK_LIB([m], [cos])

# Checks for header files.
AC_CHECK_HEADERS([float.h libintl.h limits.h locale.h stdlib.h string.h sys/ioctl.h sys/time.h termios.h unistd.h])

# Checks for typedefs, structures, and compiler characteristics.
AC_CHECK_HEADER_STDBOOL
AC_C_INLINE

# Checks for library functions.
AC_FUNC_ERROR_AT_LINE
AC_FUNC_MALLOC
AC_FUNC_STRTOD
AC_CHECK_FUNCS([alarm getcwd isascii memmove memset modf pow setlocale sqrt strcasecmp strchr strdup strncasecmp strpbrk strrchr strtol])

AC_CONFIG_FILES([makefile
                 primes/makefile])
AC_OUTPUT
