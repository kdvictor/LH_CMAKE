#链接静态链接库

cmake_minimum_required(VERSION 3.20)

project(xLog_ststic)

#指定头文件搜索路径
include_directories(xLog)

#指定链接库搜索路径
link_directories(xLog/build)

add_executable(${PROJECT_NAME} main.cpp)

#链接静态库
target_link_libraries(${PROJECT_NAME} xLog)