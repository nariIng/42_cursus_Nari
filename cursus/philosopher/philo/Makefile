NAME = philo

SRCS = 	philosopher.c	philo_utiles.c \
		exit.c 			error.c \
		init.c			action.c \
		check.c			time.c \
		fork.c			monitor.c \
		check_if.c


OBJS = $(SRCS:.c=.o)
CC = cc -Wall -Wextra -Werror
RM = rm -f

$(NAME): $(OBJS)
	@$(CC) -o $(NAME) $(OBJS)

all:$(NAME)

clean:
	@$(RM) $(OBJS)

fclean: clean
	@$(RM) $(NAME)

re: fclean all
