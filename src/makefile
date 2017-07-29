
CC := gcc
CFLAGS := -std=c11 -Wall -Wextra -Wpedantic

PROGRAM := tiger.exe


SRCS := $(wildcard *.c)
OBJS := $(patsubst %.c,%.o,$(SRCS))


$(PROGRAM): $(OBJS)
	$(CC) $(CFLAGS) -o $(PROGRAM) $(OBJS)

$(OBJS): $(SRCS)
	$(CC) $(CFLAGS) -c $(SRCS)

clean:
	rm -rf $(OBJS) $(PROGRAM)
