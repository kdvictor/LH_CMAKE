#���Ӿ�̬���ӿ�

cmake_minimum_required(VERSION 3.20)

project(xLog_ststic)

#ָ��ͷ�ļ�����·��
include_directories(xLog)

#ָ�����ӿ�����·��
link_directories(xLog/build)

add_executable(${PROJECT_NAME} main.cpp)

#���Ӿ�̬��
target_link_libraries(${PROJECT_NAME} xLog)