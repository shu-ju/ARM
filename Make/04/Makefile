# 工具链配置
CC=gcc
# 头文件位置
INC_DIRS=./inc
# 编译器选项配置
CFLAGS=-Wall -O2 -std=c99 -I$(INC_DIRS)
# 目标名称
TARGET=main
# 源文件位置
SRC_DIRS=./src

# 源文件列表
SRCS= $(SRC_DIRS)/file1.c $(SRC_DIRS)/file2.c $(SRC_DIRS)/file3.c $(SRC_DIRS)/main.c


# 编译
$(TARGET):$(SRCS:.c=.o)
	$(CC) $^ -o $@
%.o:%.c
	$(CC) $(CFLAGS) $< -c -o $@

.PHONY:clean
clean:
	rm -rf $(TARGET) $(SRCS:.c=.o)






