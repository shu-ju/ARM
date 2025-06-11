CXX=g++
CXXFLAGS= -Wall -O2 -std=c++11
SRCS=main.cc test.cc
TARGET=main

$(TARGET):$(SRCS:.cc=.o)
	$(CXX) $^ -o $@

%.o:%.cc
	$(CXX) $(CXXFLAGS) $^ -c -o $@

clean:
	rm $(TARGET) $(SRCS:.cc=.o)