# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: mcaro-ro <mcaro-ro@student.42madrid.com    +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2024/12/16 16:58:35 by mcaro-ro          #+#    #+#              #
#    Updated: 2024/12/16 17:02:56 by mcaro-ro         ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

CC = cc
CFLAGS = -Wall -Wextra -Werror

LIBDIR = ../ft_printf
LIBNAME = ftprintf

MAIN = main.c

OBJECTS = $(MAIN:.c=.o)

main: $(OBJECTS)
	$(CC) $(CFLAGS) -o out $(OBJECTS) -L$(LIBDIR) -l$(LIBNAME)
	./out

clean:
	rm -f $(OBJECTS) out

.DEFAULT_GOAL := main
.PHONY: main clean
.SILENT:
