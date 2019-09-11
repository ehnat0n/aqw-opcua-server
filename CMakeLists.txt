cmake_minimum_required(VERSION 3.14)

project(aqw-opcua-server CXX)

include(${CMAKE_BINARY_DIR}/conanbuildinfo.cmake)
conan_basic_setup(TARGETS)

add_subdirectory("aqw-opcua-server")
