AC_INIT([umem], [1.0.2], [], [umem])
AM_INIT_AUTOMAKE([dist-bzip2])

AC_PROG_CC
AM_PROG_AS
AC_PROG_LIBTOOL

AC_C_INLINE

AC_CHECK_SIZEOF(pthread_mutex_t,[],[
#include <pthread.h>
])

AC_CHECK_LIB(dl,dlopen)

AC_CHECK_HEADERS([sys/mman.h sys/sysmacros.h sys/time.h malloc.h])
AC_CHECK_FUNCS([issetugid mallinfo malloc_stats])

AC_CONFIG_HEADERS([config.h])
AC_CONFIG_FILES([Makefile Doxyfile umem.spec])

AC_OUTPUT
