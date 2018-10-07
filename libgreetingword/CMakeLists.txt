cmake_minimum_required(VERSION 3.10)
project(greetings)

set(CMAKE_CXX_STANDARD 11)

add_library(greetingword SHARED greetingword.cpp greetingword.h)

install(TARGETS greetingword DESTINATION lib)
