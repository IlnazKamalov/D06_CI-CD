executable = s21_grep
source = s21_grep.c

flags = -Wall -Werror -Wextra


all: s21_grep

s21_grep:
	gcc  $(flags) $(source) -o $(executable)

style:
	clang-format -style=Google -n -Werror *.c *.h

clean:
	rm -f *.o s21_grep

test: s21_grep
	bash test_func_grep.sh
	
rebuild: clean all
