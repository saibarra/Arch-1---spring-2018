all: out

out: bst.o
	gcc bst.o -o binarySearchTree

bst.o:	bst.c
	gcc -c bst.c

clean:
	rm bst.o binarySearchTree
