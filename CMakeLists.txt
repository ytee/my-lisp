# Specify the minimum version for CMake

cmake_minimum_required(VERSION 2.8)

# Project's name

project(my-lisp)
include_directories(inc)
file(GLOB SOURCES "src/*.c")

# Set the output folder where your program will be created
set(PROJECT_SOURCE_DIR "/home/kamakshi/Documents/GitHub/my-lisp")
set(CMAKE_BINARY_DIR ${PROJECT_SOURCE_DIR}/bin)
set(EXECUTABLE_OUTPUT_PATH ${CMAKE_BINARY_DIR})
set(LIBRARY_OUTPUT_PATH ${CMAKE_BINARY_DIR})

add_executable(repl1 ${SOURCES})
