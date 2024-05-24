# Specify the minimum CMake version
cmake_minimum_required(VERSION 3.10)

# Project name
project(backend)

# Collect all source files
set(SOURCES
    Stack.cpp
    Main.cpp
    # Add new source files here
)

# Add the library
add_library(MyBackend STATIC ${SOURCES})

# Include directories
target_include_directories(MyBackend PUBLIC include)