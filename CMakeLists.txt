cmake_minimum_required(VERSION 3.15)
project(MyProject)


set(CMAKE_EXPORT_COMPILE_COMMANDS ON)

#include(${CMAKE_BINARY_DIR}/conan_toolchain.cmake)
find_package(fmt REQUIRED)

add_executable(main main.cpp)
target_link_libraries(main fmt::fmt)


