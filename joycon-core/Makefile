CC = g++ -std=c++14
FLAGS = -march=native -Wall -g -rdynamic
LIBS	= -I/usr/local/include -L/usr/local/lib -lhidapi-hidraw -pthread

A_SRC = joycon-core.cpp
A_TARGET = libjoycon-core.so

.PHONY: libjoycon-core.so
joycon-core.so: $(A_SRC)
	$(CC) $(A_SRC) $(FLAGS) $(LIBS) -shared -fPIC -o $(A_TARGET)
		@echo "> Compiled joycon-core.so"
