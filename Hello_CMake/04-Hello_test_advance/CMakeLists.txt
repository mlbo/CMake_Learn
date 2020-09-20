cmake_minimum_required(VERSION 3.16)

#The project name
project(hello_cmake)

# The source shared between the main program and the tests
set(PROJECT_SOURCES hello.cpp hello.h)

# The main program
add_executable(prog main.cpp ${PROJECT_SOURCES})

# The test
add_executable(tests testmain.cpp ${PROJECT_SOURCES})
