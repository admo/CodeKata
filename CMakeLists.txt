cmake_minimum_required(VERSION 3.7)
project(PrimeFactorsKata)

set(CMAKE_CXX_STANDARD 14)

add_library(CodeKata OBJECT CodeKata.cpp)

add_subdirectory(tests)
