LEX = flex
YACC = bison

all:
	$(LEX) -o token.c token.l
	$(YACC) -d -o grammer.c grammer.y
	gcc -o parser grammer.c token.c main.c

clean:
	rm grammer.[ch]
	rm token.c 
