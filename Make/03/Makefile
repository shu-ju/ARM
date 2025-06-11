# 工具链配置
CXX = aarch64-none-linux-gnu-g++

# 头文件列表
INC_DIRS = ./dir

# 编译选项配置
CXXFLAGS = -Wall -O2 -std=c++11 -I$(INC_DIRS)

# 目标名称 
TARGET = main

# 源文件列表
SRCS = main.cc sort.cc foo.cc


# 编译
$(TARGET):$(SRCS:.cc=.o)
	$(CXX) $^ -o $@

%.o:%.cc
	$(CXX) $(CXXFLAGS) $^ -o $@ -c


.PHONY:clean
clean:
	rm -rf $(TARGET) $(SRCS:.cc=.o)