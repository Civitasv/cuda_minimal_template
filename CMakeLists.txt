cmake_minimum_required(VERSION 3.16)

################### Enable cuda #######################
set(CMAKE_CUDA_COMPILER /usr/local/cuda-12.1/bin/nvcc)
enable_language("CUDA")
#######################################################

project(cuda-minimal)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED TRUE)

add_subdirectory(vendor)
add_subdirectory(src)
add_subdirectory(tests)
