# SPDX-License-Identifier: GPL-2.0+

AUTOMAKE_OPTIONS = foreign
bin_PROGRAMS     = erofsfuse
erofsfuse_SOURCES = main.c
erofsfuse_CFLAGS = -Wall -Werror -I$(top_srcdir)/include
erofsfuse_CFLAGS += -DFUSE_USE_VERSION=26 ${libfuse_CFLAGS} ${libselinux_CFLAGS}
erofsfuse_LDADD = $(top_builddir)/lib/liberofs.la ${libfuse_LIBS} ${liblz4_LIBS} \
	${libselinux_LIBS} ${liblzma_LIBS}
