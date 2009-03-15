# Copyright (C) 2005, 2006, 2007 Giuseppe Martino <denever@users.sf.net>
#
# This file is free software; as a special exception the author gives
# unlimited permission to copy and/or distribute it, with or without 
# modifications, as long as this notice is preserved.
# 
# This program is distributed in the hope that it will be useful, but
# WITHOUT ANY WARRANTY, to the extent permitted by law; without even the
# implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.

bin_PROGRAMS = shell-fm
shell_fm_SOURCES = autoban.c bookmark.c completion.c feeds.c getln.c hash.c history.c http.c interface.c main.c md5.c mix.c pipe.c play.c playlist.c radio.c readline.c recommend.c ropen.c sckif.c service.c settings.c split.c strary.c submit.c tag.c util.c xmlrpc.c
shell_fm_LDADD = $(AO_LIBS) $(MAD_LIBS)
INCLUDES = -I$(top_srcdir)/include $(AO_CFLAGS) $(MAD_CFLAGS)
