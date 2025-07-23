$(VERBOSE).SILENT:

all: output main.o clean

output: main.o
	gcc main.o -L./lib/ -lMY -o program.exe
	echo "Program has been compiled successfully..."

main.o: main.c
	gcc -c main.c -I./lib/

uninstall:
	rm -rf program.exe

clean:
	rm -rf *.o

