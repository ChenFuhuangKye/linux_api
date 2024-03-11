CC=gcc

CFLAGS=-g -Wall

TARGET=tim_sort

$(TARGET): main.o timsort.o 
	$(CC) $(CFLAGS) -o $(TARGET) main.o timsort.o 

main.o: main.c sort_impl.h
	$(CC) $(CFLAGS) -c main.c

timsort.o: timsort.c sort_impl.h list.h
	$(CC) $(CFLAGS) -c timsort.c

clean:
	rm -f $(TARGET) *.o