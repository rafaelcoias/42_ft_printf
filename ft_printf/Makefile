# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: rade-sar <marvin@42.fr>                    +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2021/12/16 16:25:52 by rade-sar          #+#    #+#              #
#    Updated: 2021/12/16 16:33:55 by rade-sar         ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

SRC = ./ft_printf.c ./ft_putchar.c ./ft_putstr.c ./ft_putnbr.c ./ft_putvoid.c ./ft_puthexa.c

OBJ = ${SRC:.c=.o}

NAME = libftprintf.a

HEAD = includes

GCC = gcc

FLAGS = -Wall -Wextra -Werror

RM = rm -f

AR = ar rcs

RANLIB = ranlib

.c.o:
		${GCC} ${FLAGS} -c $< -o ${<:.c=.o} -I ${HEAD}

${NAME}:${OBJ}
		${AR} ${NAME} ${OBJ}
		${RANLIB} ${NAME}

all: 	${NAME}

clean: 
		${RM} ${OBJ}

fclean:	clean
		${RM} ${NAME}

re:		fclean all

norm:
		norminette -R CheckForbiddenSourceHeader *.c
		norminette -R CheckDefine *.h
