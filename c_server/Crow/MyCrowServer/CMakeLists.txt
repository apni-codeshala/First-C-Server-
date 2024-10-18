cmake_minimum_required(VERSION 3.10)
project(MyCrowServer)

set(CMAKE_CXX_STANDARD 11)

# Specify the path to the Crow library
add_subdirectory(../Crow Crow)

add_executable(MyCrowServer main.cpp)
target_link_libraries(MyCrowServer PRIVATE Crow::crow)
