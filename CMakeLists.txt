cmake_minimum_required(VERSION "3.21.0")

#Set target output directory
set(CMAKE_ARCHIVE_OUTPUT_DIRECTORY "${CMAKE_BINARY_DIR}/lib")
set(CMAKE_LIBRARY_OUTPUT_DIRECTORY "${CMAKE_BINARY_DIR}/lib")
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY "${CMAKE_BINARY_DIR}/lib")

option(BUILD_SHARED_LIBS "True when building a shared library" True)

project("Foo")

add_subdirectory("foo")

add_subdirectory("examples")