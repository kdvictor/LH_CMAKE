#链接静态链接库

cmake_minimum_required(VERSION 3.20)

project(xLog_shared)

#指定头文件搜索路径
include_directories(xLog)

add_library(xLog SHARED xLog/xLog.cpp)

#指定链接库搜索路径
link_directories(out/build)

add_executable(${PROJECT_NAME} MAIN/main.cpp)

#链接静态库
target_link_libraries(${PROJECT_NAME} xLog)