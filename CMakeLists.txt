cmake_minimum_required(VERSION 3.10.2)

set(PROJECT learnZinx)
project(${PROJECT})

set(CMAKE_CXX_STANDARD 17)

#include_directories(/home/cyd/project/zinx) # 引入动态库;make install后，zinx.h在usr/bin/include
#link_directories(/usr/bin/) # 引入动态库；默认路径不需要单独声明了

add_executable(${PROJECT} main.cpp)
target_link_libraries(${PROJECT} -lzinx) # 引入动态库

