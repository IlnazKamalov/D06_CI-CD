executable = s21_cat
source = s21_cat.c

flags = -Wall -Werror -Wextra

all: build

build: s21_cat

s21_cat: 
	gcc $(flags) $(source) -o $(executable)

style:
	clang-format -style=Google -n -Werror *.c

test:
	bash t_cat.sh

clean:
	rm -f $(executable) *.o
