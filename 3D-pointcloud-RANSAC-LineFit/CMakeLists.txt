cmake_minimum_required(VERSION 2.8 FATAL_ERROR)

project(lineFit)

find_package(PCL 1.8 REQUIRED)

include_directories(${PCL_INCLUDE_DIRS})
link_directories(${PCL_LIBRARY_DIRS})
add_definitions(${PCL_DEFINITIONS})

add_executable (lineFit main.cpp)
target_link_libraries (lineFit ${PCL_LIBRARIES})
