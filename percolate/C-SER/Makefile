MF=	Makefile

CC=	icc
CFLAGS=	-O3

LFLAGS= $(CFLAGS)

EXE=	percolate

INC= \
	percolate.h

SRC= \
	percolate.c \
	percwrite.c \
	uni.c

#
# No need to edit below this line
#

.SUFFIXES:
.SUFFIXES: .c .o

OBJ=	$(SRC:.c=.o)

.c.o:
	$(CC) $(CFLAGS) -c $<

all:	$(EXE)

$(OBJ):	$(INC)

$(EXE):	$(OBJ)
	$(CC) $(LFLAGS) -o $@ $(OBJ)

$(OBJ):	$(MF)

clean:
	rm -f $(EXE) $(OBJ) core
