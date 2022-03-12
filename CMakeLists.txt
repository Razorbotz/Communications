cmake_minimum_required(VERSION 3.0.0)
project(communications LANGUAGES CXX)

# Language options
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_C_STANDARD 11)

# Compiler options
set(CMAKE_CXX_FLAGS "-Wall -Wextra -pedantic")
set(CMAKE_CXX_FLAGS_DEBUG "-g")
set(CMAKE_CXX_FLAGS_RELEASE "-O2")

# Source options
include_directories(include)

# Target Options
add_library(${CMAKE_PROJECT_NAME} STATIC src/communications.cpp)
