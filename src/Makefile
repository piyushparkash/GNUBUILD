hw: main.o libhello.a
	cc -o hw main.o libhello.a

libhello.a: hello.o
	ar cru libhello.a hello.o
	ranlib libhello.a

.SUFFIXES: .c .o

.c.o:
	cc -c -o $@ $<

clean:
	rm -f hw main.o hello.o libhello.a