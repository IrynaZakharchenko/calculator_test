cmake_minimum_required(VERSION 3.0)

set(CMAKE_CXX_STANDARD 11)

project(calculator)

find_package(GTest REQUIRED)

set(SOURCES calculator.cpp)
add_executable(calculator_test calculator_test.cc ${SOURCES})

target_link_libraries(calculator_test gtest gmock_main)
