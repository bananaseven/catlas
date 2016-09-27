cmake_minimum_required(VERSION 3.6)
project(Catlas)

#set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")

#set(SOURCE_FILES main.c)

#add_executable(Catlas_esp8266 ${SOURCE_FILES} esp8266_main.c)
add_executable(Catlas_tests ${SOURCE_FILES} test_main.c)