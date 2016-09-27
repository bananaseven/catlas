cmake_minimum_required(VERSION 3.6)
project(Catlas)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")


set(SOURCE_FILES Catlas.c)
add_library(catlas ${SOURCE_FILES})
