TESTROOT = ../..
include ${TESTROOT}/include/common.makefile

#
# verify addends work
#

all-check: all check

check:
	./main 
	 
all:

	${CC} ${CCFLAGS} foo.c abs.s -dynamiclib -o libfoo.dylib 
	${CC} ${CCFLAGS} -I${TESTROOT}/include libfoo.dylib -o main main.c


clean:
	${RM} ${RMFLAGS} *~ main  libfoo.dylib

