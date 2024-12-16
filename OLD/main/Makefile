CC = cc
CFLAGS = -Wall -Wextra -Werror
DIR = -I$(LIBDIR)

LIBDIR = ../ft_printf
LIBNAME = ftprintf

MAIN = main.c

MOBJECTS = $(MAIN:.c=.o)

main: $(MOBJECTS)
	$(CC) $(CFLAGS) $(DIR) -o out $(MOBJECTS) -L$(LIBDIR) -l$(LIBNAME)
	./out

mclean:
	rm -f $(MOBJECTS) out

.DEFAULT_GOAL := main

.PHONY: main mclean
.SILENT:
