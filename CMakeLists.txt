cmake_minimum_required(VERSION 3.23)
project(CUDA_GRAPHS CUDA)

set(CMAKE_CUDA_STANDARD 14)

add_executable(CUDA_GRAPHS main.cu graphs.cuh graphs.cu)

set_target_properties(CUDA_GRAPHS PROPERTIES
        CUDA_SEPARABLE_COMPILATION ON)
