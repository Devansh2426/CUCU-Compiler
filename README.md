# CUCU-compiler

----------------------------
Project Name: CUCU Compiler

Files:
	cucu.l: Lexer file written in Flex.
	cucu.y: Parser file written in Bison.
	sample1.cu: Sample input file in the custom language which is syntactically correct.
	sample2.cu: Sample input file in the custom language which is syntactically incorrect.

To Run the Program:
	flex cucu.l
	yacc -d cucu.y
	cc lex.yy.c cucu.tab.c -o cucu
	./cucu (input_file.cu)