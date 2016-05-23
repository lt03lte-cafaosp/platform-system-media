AM_CFLAGS = -Werror -Wall

pkgconfigdir = $(libdir)/pkgconfig
pkgconfig_DATA = tinysndfile.pc
EXTRA_DIST = $(pkgconfig_DATA)

AM_CFLAGS += -I $(WORKSPACE)/system/media/audio_utils
AM_CFLAGS += -I $(WORKSPACE)/system/media/audio_utils/include

library_includedir = $(includedir)/tinysndfile
library_include_HEADERS = include/audio_utils/sndfile.h

c_sources = tinysndfile.c \
            primitives.c

lib_LTLIBRARIES = libtinysndfile.la
libtinysndfile_la_SOURCES = $(c_sources)
libtinysndfile_la_CFLAGS = $(AM_CFLAGS)
