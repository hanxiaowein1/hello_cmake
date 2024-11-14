cmake_minimum_required(VERSION 3.10.0)

set(CMAKE_CXX_STANDARD 20)

set(CMAKE_PREFIX_PATH "D:\\OwnLibrary" ${CMAKE_PREFIX_PATH})

project(cmake_exe0)

add_executable(${PROJECT_NAME} main.cpp)

find_package(cmake_lib0)

target_link_libraries(${PROJECT_NAME} cmake_lib0::cmake_lib0)