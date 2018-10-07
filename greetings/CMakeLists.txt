cmake_minimum_required(VERSION 3.10)
project(greetings)

set(CMAKE_CXX_STANDARD 11)

include_directories(../libgreetingword)

add_executable(greetings main.cpp)

target_link_libraries(greetings greetingword)
