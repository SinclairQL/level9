# Makefile - QDOS  Level9 Makefile
# Copyright (c) 2017, tcat <thomas.kral@email.cz>

# This program is free software; you can redistribute it and/or modify
# it under the terms of the GNU General Public License as published by
# the Free Software Foundation; either version 2 of the License, or
# (at your option) any later version.
#
# This program is distributed in the hope that it will be useful,
# but WITHOUT ANY WARRANTY; without even the implied warranty of
# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
# GNU General Public License for more details.
#
# You should have received a copy of the GNU General Public License
# along with this program; if not, write to the Free Software
# Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111, USA.

#######################################################################

CC = qdos-gcc
OBJS = level9.o bitmap.o ql.o
CFLAGS = -Wall
LFLAGS = -lm
RM = rm -f
LIBS = 

level9: $(OBJS)
	$(CC) -o level9 $(OBJS) $(LIBS) $(LFLAGS) 

clean:
	$(RM) level9 *.o

level9.o:
	$(CC) -c $(CFLAGS) level9.c
bitmap.o:
	$(CC) -c $(CFLAGS) bitmap.c
ql.o:
	$(CC) -c $(CFLAGS) ql.c

level9.o: level9.h level9.c
bitmap.o: bitmap.c
ql.o:     ql.c


# end of Makefile
