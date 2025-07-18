NAME = philo

CC = gcc
CFLAGS = -Wall -Wextra -Werror -pthread

SRC = main.c utils.c init.c threads.c monitor.c routine_actions.c
OBJ = $(SRC:.c=.o)

all: $(NAME)

$(NAME): $(OBJ)
	$(CC) $(CFLAGS) $(OBJ) -o $(NAME)

clean:
	rm -f $(OBJ)

fclean: clean
	rm -f $(NAME)

re: fclean all

.PHONY: all clean fclean re