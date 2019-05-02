cmake_minimum_required(VERSION 3.12)

project(LibraryExperiment C CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)
set(CMAKE_POSITION_INDEPENDENT_CODE ON)     # for fpic

set(CMAKE_RUNTIME_OUTPUT_DIRECTORY bin)

add_subdirectory(libraries)
add_subdirectory(sample_app)