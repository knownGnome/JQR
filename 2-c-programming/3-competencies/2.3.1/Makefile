CC = gcc
CFLAGS = -g -Wall -Wextra


run: main
	valgrind ./main

main: main.c start.o
	$(CC) $(CFLAGS) $^ -o $@

start.o: start.c
	$(CC) $(CFLAGS) -c $^ -o $@

clean:
	rm -f *.o main

.PHONY: run clean