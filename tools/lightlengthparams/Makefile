all : lightlengthparams

SRT:=../..

LIBSURVIVE:=$(SRT)/lib/libsurvive.so

CFLAGS:=-I$(SRT)/redist -I$(SRT)/include -O0 -g -DFLT=double -DUSE_DOUBLE
LDFLAGS:=-lm -lpthread -llapacke  -lcblas 

lightlengthparams : lightlengthparams.c $(LIBSURVIVE) 
	gcc $(CFLAGS) -o $@ $^ $(LDFLAGS)

clean :
	rm -rf lightlengthparams

