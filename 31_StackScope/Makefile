CXX = g++

# Warnings frequently signal eventual errors:
CXXFLAGS=-g -std=c++14 -W -Wall -Wextra -pedantic -O0

OBJS = \
	./src/main.o
EXEC = run

%.o: %.cpp
	$(CXX) $(CXXFLAGS) -c $< -o $@

$(EXEC): $(OBJS)
	$(CXX) $(CXXFLAGS) -o $@ $(OBJS) $(LDFLAGS)

main.o: main.cpp

clean:
	rm -rf $(OBJS)
	rm -rf $(EXEC)
