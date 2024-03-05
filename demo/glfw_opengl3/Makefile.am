##
## Description  : NUKLEAR-TEMPLATES - Makefile.am
## Author       : DRE 2024
## Purpose      : main Makefile
## Revision     : $Id: Makefile.am,v 1.12 2008/12/02 20:49:08 cvsuser Exp $
##
# added old Makefile as add-on that allows backwards compatability to original Makefile recipes.
include "Makefile.old"

# DRE 2022 : the subdirectories alert for automake 
# NOTE: Every line ends in a Carriage Return
SUBDIRS = 

# DRE2022 - a generic aclocal flag set for m4 files
ACLOCAL_AMFLAGS = -I m4 -I/usr/include -I/usr/local/include


# DRE 2022: test programs for the library straight from Michael Kerrisk's examples:
check_PROGRAMS			= test-demo 

# DRE 2022: Become a Nuklear check target
test_demo_SOURCES						=  main.c
test_demo_CFLAGS						=  -std=c99 -pedantic -O2
test_demo_LDFLAGS						=  $(GLFW3) -lGL -lm -lGLU -lGLEW


# DRE 2022 - target recipe makes doxygen outputs, after updating config format file
dox:
	doxygen
	



##############################################################################
#
# ORIGINAL NUKLEAR MAKEFILE
#
###############################################################################
# Install
#BIN = demo

# Flags
#CFLAGS += -std=c99 -pedantic -O2

#SRC = main.c
#OBJ = $(SRC:.c=.o)

#ifeq ($(OS),Windows_NT)
#BIN := $(BIN).exe
#LIBS = -lglfw3 -lopengl32 -lm -lGLU32 -lGLEW32
#else
#	UNAME_S := $(shell uname -s)
#	GLFW3 := $(shell pkg-config --libs glfw3)
#	ifeq ($(UNAME_S),Darwin)
#		LIBS := $(GLFW3) -framework OpenGL -framework Cocoa -framework IOKit -framework CoreVideo -lm -lGLEW -L/usr/local/lib
#	else
#		LIBS = $(GLFW3) -lGL -lm -lGLU -lGLEW
#	endif
#endif

#$(BIN):
#	@mkdir -p bin
#	rm -f bin/$(BIN) $(OBJS)
#	$(CC) $(SRC) $(CFLAGS) -o bin/$(BIN) $(LIBS)
