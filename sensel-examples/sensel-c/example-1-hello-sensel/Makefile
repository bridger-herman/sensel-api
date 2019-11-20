NAME = hellosensel

SRC = main.c

SRCPRFX = $(addprefix src/, $(SRC))

OBJ = $(SRCPRFX:.c=.o)

OBJPRFX = build/

INCLDIR = ../../../sensel-lib/src

CC = gcc

CFLAGS = -c -std=c99 -Wall -Werror -O2

LDFLAGS = -lsensel 

all: cleanobj $(OBJ)
	mkdir -p $(OBJPRFX)/obj
	mv $(OBJ) $(OBJPRFX)/obj
	$(CC) -I $(INCLDIR) $(addprefix $(OBJPRFX)/obj/, $(notdir $(OBJ))) -o $(addprefix $(OBJPRFX), $(NAME)) $(LDFLAGS)

clean: cleanobj
	rm -rf build/

cleanobj:
	rm -f src/*.o
