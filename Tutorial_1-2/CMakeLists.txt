cmake_minimum_required(VERSION 3.10)

project(Tutorial_1)

add_executable(${PROJECT_NAME} main.cpp)

add_subdirectory(Adder)

target_link_directories(${PROJECT_NAME} PRIVATE adder)


target_link_libraries(${PROJECT_NAME} adder)