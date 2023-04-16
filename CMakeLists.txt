
cmake_minimum_required(VERSION 3.3)

PROJECT(test)
#set(Eigen3_DIR D:/ProgramFiles/Eigen3/share/eigen3/cmake)


message("nihao${EIGEN3_INCLUDE_DIR}")
add_executable(test main.cpp)
#include_directories(${CMAKE_CURRENT_SOURCE_DIR}/extern/Eigen/include/eigen3)

target_include_directories(test PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}/extern/Eigen/include/eigen3)