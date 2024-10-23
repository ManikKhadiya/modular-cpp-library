cmake_minimum_required(VERSION 3.10)
project(ModularCppLibrary)

set(CMAKE_CXX_STANDARD 17)

include_directories(include)

file(GLOB_RECURSE SOURCES "src/**/*.cpp")

add_library(modular_cpp STATIC ${SOURCES})

enable_testing()
add_subdirectory(tests)
