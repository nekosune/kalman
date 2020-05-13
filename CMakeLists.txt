cmake_minimum_required(VERSION 3.16)
# cmake_minimum_required(VERSION <specify CMake version here>)
project(kalman)

set(CMAKE_CXX_STANDARD 14)
add_subdirectory(Eigen)
add_executable(kalman main.cpp measurement_package.h tracking.h tracking.cpp kalman_filter.h kalman_filter.cpp)