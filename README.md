ex1: exemplo.o 
	gcc exemplo.o  -o teste

ex1.o: exemplo.c
	gcc -c exemplo.c 

clean:
	rm *.o
