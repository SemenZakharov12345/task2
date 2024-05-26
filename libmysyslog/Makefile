CC = gcc
CFLAGS = -Wall -Wextra -fPIC
TARGET = libmysyslog.so

all: $(TARGET)

$(TARGET): libmysyslog.o
	$(CC) -shared -o $(TARGET) libmysyslog.o

libmysyslog.o: libmysyslog.c libmysyslog.h
	$(CC) $(CFLAGS) -c $<

clean:
	rm -f $(TARGET) *.o

.PHONY: all clean
