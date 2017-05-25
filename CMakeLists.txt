cmake_minimum_required(VERSION 3.7)
project(c)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11 -fPIC")
set(SOURCE_FILES libraryC.cpp libraryC.h)
link_directories("/Users/raoshaoquan/CLionProjects/c/lib")
add_library(c SHARED  ${SOURCE_FILES})
target_link_libraries(c a)