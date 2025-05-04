CFLAGS ?= -Wall -DMAIN
CXXFLAGS ?= -Wall -std=c++11

.PHONY: all clean
all: decompile compile extract

decompile: decompile.cc
decompile.cc: fonttable.h opcodes.h

compile: compile.cc
compile.cc: rfonttable.h ropcodes.h

extract: extract.c
extract.c: extract.h

clean:
	rm -f extract compile decompile
