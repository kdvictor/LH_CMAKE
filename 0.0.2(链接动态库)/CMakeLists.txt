#���Ӿ�̬���ӿ�

cmake_minimum_required(VERSION 3.20)

project(xLog_shared)

#ָ��ͷ�ļ�����·��
include_directories(xLog)

add_library(xLog SHARED xLog/xLog.cpp)

#ָ�����ӿ�����·��
link_directories(out/build)

add_executable(${PROJECT_NAME} MAIN/main.cpp)

#���Ӿ�̬��
target_link_libraries(${PROJECT_NAME} xLog)