# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: jdeclan <jdeclan@student.21-school.ru>     +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2021/11/10 16:17:10 by jdeclan           #+#    #+#              #
#    Updated: 2021/11/14 18:39:44 by jdeclan          ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

NAME	= libft.a
HEADER	= libft.h
CC		= cc
CFLAGS	= -Wall -Wextra -Werror
RM		= rm -rf

LIST	= ft_isalpha.c		ft_isdigit.c		ft_isalnum.c\
		ft_isascii.c		ft_isprint.c		ft_strlen.c\
		ft_memset.c			ft_bzero.c			ft_memcpy.c\
		ft_memmove.c		ft_strlcpy.c		ft_strlcat.c\
		ft_toupper.c		ft_tolower.c		ft_strchr.c\
		ft_strrchr.c		ft_strncmp.c		ft_memchr.c\
		ft_memcmp.c			ft_strnstr.c		ft_atoi.c\
		ft_calloc.c			ft_strdup.c			ft_substr.c\
		ft_strjoin.c		ft_strtrim.c		ft_split.c\
		ft_itoa.c			ft_strmapi.c		ft_putchar_fd.c\
		ft_putstr_fd.c		ft_putendl_fd.c		ft_putnbr_fd.c\
		ft_striteri.c

OBJS = $(LIST:.c=.o)

all: $(NAME)

$(NAME): $(OBJS)
	ar rcs $(NAME) $?

%.o: %.c $(HEADER)
	$(CC) $(CFLAGS) -c $<

clean:
	@$(RM) $(OBJS)

fclean: clean
	@$(RM) $(NAME)

re: fclean all

.PHONY: all re clean fclean
