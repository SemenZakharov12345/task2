CC = gcc
CFLAGS = -Wall -Werror -fPIC
LDFLAGS = -shared
TARGET = libmysyslog.so

all: $(TARGET)

$(TARGET): libmysyslog.o
	$(CC) $(LDFLAGS) -o $@ $^

libmysyslog.o: libmysyslog.c libmysyslog.h
	$(CC) $(CFLAGS) -c $<

clean:
	rm -f *.o $(TARGET)

.PHONY: all clean
