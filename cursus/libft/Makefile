NAME = libft.a

SRCS = 	ft_atoi.c ft_isdigit.c ft_memmove.c ft_split.c ft_strlcat.c \
		ft_strtrim.c ft_bzero.c ft_isprint.c ft_memset.c ft_strchr.c \
		ft_strlcpy.c ft_substr.c ft_calloc.c ft_itoa.c ft_putchar_fd.c \
		ft_strcmp.c ft_strlen.c ft_tolower.c ft_isalnum.c ft_memchr.c \
		ft_putendl_fd.c ft_strdup.c ft_strmapi.c ft_toupper.c ft_isalpha.c \
		ft_memcmp.c   ft_putnbr_fd.c   ft_striteri.c  ft_strnstr.c ft_strncmp.c\
		ft_isascii.c ft_memcpy.c ft_putstr_fd.c ft_strjoin.c ft_strrchr.c

SRCS_B = 	ft_lstnew_bonus.c ft_lstadd_front_bonus.c ft_lstsize_bonus.c \
			ft_lstlast_bonus.c ft_lstadd_back_bonus.c ft_lstdelone_bonus.c \
			ft_lstclear_bonus.c ft_lstiter_bonus.c ft_lstmap_bonus.c
	
CC = cc

CFLAGS = -Wall -Wextra -Werror

LIBC = ar -rcs

RM = rm -f

INCS = libft.h

OBJS = $(SRCS:.c=.o)

OBJS_B = $(SRCS_B:.c=.o)

.c.o :
	$(CC) $(CFLAGS) -c $< -o $(<:.c=.o) -I $(INCS)

$(NAME) : $(OBJS)
	$(LIBC) $(NAME) $(OBJS)

bonus : $(OBJS) $(OBJS_B)
	$(LIBC) $(NAME) $(OBJS) $(OBJS_B)
	
all : $(NAME)

clean :
	$(RM) $(OBJS) $(OBJS_B)

fclean : clean
	$(RM) $(NAME)

re : fclean all

.PHONY : all bonus clean fclean re
