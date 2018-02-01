all: hello string



hello:	hello.o
	gcc hello.o -o hello

hello.o: 	
	gcc -c hello.c


string: string.o
	gcc string.o -o string

string.o: nameCompareFile.c
	gcc -c nameCompareFile.c


clean:
	rm hello.o hello string.o string

