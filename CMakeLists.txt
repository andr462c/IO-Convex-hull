cmake_minimum_required(VERSION 3.0)

project(convex-hull)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++17 -Wno-dev -O3")

add_subdirectory(graham-scan)

add_executable(convex-hull main.cpp)
target_link_libraries(convex-hull graham-scan)