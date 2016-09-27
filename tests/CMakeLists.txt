cmake_minimum_required(VERSION 3.6)
project(Catlas_test)

add_subdirectory(lib/gtest-1.7.0)
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")
#set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c99")
include_directories(${gtest_SOURCE_DIR} ${gtest_SOURCE_DIR}/include)

set(SOURCE_FILES build_test.cpp)
add_executable(Catlas_test ${SOURCE_FILES})

target_link_libraries(Catlas_test catlas gtest gtest_main)
