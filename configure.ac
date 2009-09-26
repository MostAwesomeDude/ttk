AC_INIT([TTK], [0.1])
AM_INIT_AUTOMAKE([-Wall -Werror foreign])
LT_INIT

AC_PROG_CC
AC_PROG_LEX
AC_PROG_LIBTOOL

PKG_CHECK_MODULES([PNG], [libpng])

AM_PATH_SDL
CFLAGS="$CFLAGS $SDL_CFLAGS $PNG_CFLAGS"
LIBS="$LIBS $SDL_LIBS $PNG_LIBS"

AC_CONFIG_FILES([Makefile src/Makefile include/Makefile
    examples/Makefile ttk.pc])

AC_OUTPUT
