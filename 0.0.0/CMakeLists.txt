#第一个cmake构建的程序

#指定cmake最低版本
cmake_minimum_required(VERSION 3.20)

#设置构建项目的名称
project(first_cmake)

#构建执行程序
add_executable(${PROJECT_NAME} first_cmake.cpp)