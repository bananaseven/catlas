cmake_minimum_required(VERSION 3.6)
project(Catlas_run_proj)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")


set(SOURCE_FILES catlas/Catlas.c)
add_executable(Catlas_run ${SOURCE_FILES} main.c)

include_directories(catlas)

add_subdirectory(tests)
add_subdirectory(catlas)

target_link_libraries(Catlas_run catlas)