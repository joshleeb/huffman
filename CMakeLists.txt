cmake_minimum_required(VERSION 3.7)
project(huffman)

set(CMAKE_BUILD_TYPE Debug)
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++14 -Wall -Werror")

file(GLOB_RECURSE SOURCES src/*.cc src/*.h)

add_executable(huffman src/main.cc ${SOURCES})