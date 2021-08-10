cmake_minimum_required(VERSION 3.17)
project(JsonTutorial)

set(CMAKE_CXX_STANDARD 11)

add_library(leptjson leptjson.c)

#add_executable(JsonTutorial main.cpp leptjson.cpp leptjson.h test.c)
add_executable(JsonTutorial test.c )
target_link_libraries(JsonTutorial leptjson)