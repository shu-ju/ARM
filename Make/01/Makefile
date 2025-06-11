CXX=g++
CXXFLAGS= -Wall -O2 -std=c++11
SRCS=main.cc test.cc
OBJS=main.o test.o
TARGET=main

$(TARGET):$(OBJS)
	$(CXX) $^ -o $@
%.o:%.cc
	$(CXX) $(CXXFLAGS) $< -c -o $@
clean:
	rm $(TARGET) $(OBJS)