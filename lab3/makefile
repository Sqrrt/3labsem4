memfunc: lab3_memfunc.c
	gcc -c lab3.c
	ar rc liblab3.a lab3.o
	ranlib liblab3.a
	gcc  -g -pthread lab3_memfunc.c -L -llab3 -o lab3_memfunc
main: lab3_main.c
	gcc -c lab3_memfunc.c
	ar rc liblab3_memfunc.a lab3_memfunc.o
	ranlib liblab3_memfunc.a
	gcc -g -pthread lab3_main.c -L -llab3_memfunc -o lab3_main
clean:
	rm -rf lab3_memfunc lab3_main *.o *.out *.a
