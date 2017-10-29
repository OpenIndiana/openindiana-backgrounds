dnl Process this file with autoconf to produce a configure script.

AC_PREREQ([2.63])
AC_INIT([openindiana-backgrounds],
        [1.0],
        [https://bugs.launchpad.net/openindiana],
        [openindiana-backgrounds],
        [http://openindiana.org/])
AM_INIT_AUTOMAKE([foreign tar-ustar dist-bzip2])
AM_MAINTAINER_MODE
AC_CONFIG_SRCDIR([data/openindiana-backgrounds.xml.in.in])

AC_PROG_INSTALL
AC_PROG_SED
IT_PROG_INTLTOOL([0.40.0])

GETTEXT_PACKAGE=openindiana-backgrounds
AC_SUBST(GETTEXT_PACKAGE)
AC_DEFINE_UNQUOTED(GETTEXT_PACKAGE,
                   "${GETTEXT_PACKAGE}",
                   [the gettext translation domain])
AM_GNU_GETTEXT([external])
AM_GNU_GETTEXT_VERSION([0.17])

AC_CONFIG_HEADERS([config.h])
AC_CONFIG_FILES([Makefile
        po/Makefile.in
        data/Makefile])
AC_OUTPUT

