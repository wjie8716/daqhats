NAME = finite_scan_with_trigger
OBJ = $(NAME).o
LIBS = -ldaqhats
CFLAGS = -Wall -I/usr/local/include -g
CC = gcc
EXTENSION = .c

all: $(NAME)

%.o: %$(EXTENSION) $(DEPS)
	$(CC) -c -o $@ $< $(CFLAGS)

$(NAME): $(OBJ)
	$(CC) -o $@ $^ $(CFLAGS) $(LIBS)

.PHONY: clean

clean:
	@rm -f *.o *~ core $(NAME) test.csv
