CC := gcc
SRC_PATH := ./src
INCLUDE_PATH := ./include
SRC := $(SRC_PATH)/*.c
FILENAME := ssu_lsproc

INCLUDE_OPT := -I $(INCLUDE_PATH)
LIBRARY_OPT := -lm
RENAME_OPT := -o ./output/$(FILENAME)
DEBUG_OPT := -DDEBUG -g
OPT:=$(RENAME_OPT) $(INCLUDE_OPT) $(LIBRARY_OPT) -W -Wall

all : src include
	$(CC) $(SRC) $(OPT)

debug : src include
	$(CC) $(SRC) $(OPT) $(DEBUG_OPT)

clear : output
	rm ./output/$(FILENAME)
