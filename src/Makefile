# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: aeddaoud <marvin@42.fr>                    +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2021/12/08 13:10:44 by aeddaoud          #+#    #+#              #
#    Updated: 2021/12/08 13:10:57 by aeddaoud         ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

SRC=ft_printf.c ft_utils.c
CC=cc
FLAGS=-Wall -Werror -Wextra -c
O_SRC=$(SRC:%.c=%.o)
NAME=libftprintf.a

all: $(NAME)

$(NAME): $(O_SRC)

%.o:%.c
	$(CC) $(FLAGS) $<
	ar -rc $(NAME) $@

clean:
	rm -rf *.o

fclean: clean
	rm -rf $(NAME)

re: fclean all
