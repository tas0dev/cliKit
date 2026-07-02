cmake_minimum_required(VERSION 4.2)
project(cliKit C)

set(CMAKE_C_STANDARD 99)

add_library(cliKit STATIC src/clikit.c)

add_executable(examples examples/test.c)
target_link_libraries(examples cliKit)
