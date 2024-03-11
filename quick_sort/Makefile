CC=gcc

CFLAGS=-g -Wall

TARGET=quick_sort

$(TARGET): main.o node.o
	$(CC) $(CFLAGS) -o $(TARGET) main.o node.o

main.o: main.c node.h
	$(CC) $(CFLAGS) -c main.c

node.o: node.c node.h
	$(CC) $(CFLAGS) -c node.c

clean:
	rm -f $(TARGET) main.o node.o
