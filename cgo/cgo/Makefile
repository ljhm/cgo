# build shared library with -fPIC, -shared
CFLAGS   = -Wall -Wextra -g -std=c99 -fPIC # -O3   # CXXFLAGS for .cpp
LDFLAGS  = -shared # -L../hello
LDLIBS   = # -lhello
CPPFLAGS = -MMD -MP # -I../hello
# CC      = $(CXX)  # link with CXX for .cpp

# target name is basename of one of the source files
cgo : $(patsubst %.c,%.o,$(wildcard *.c))  # .cpp
-include *.d
clean : ; -rm -fr *.o *.d
.PHONY : clean
