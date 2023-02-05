cmake_minimum_required(VERSION 3.13)
project(cgltf)
set(CMAKE_CXX_STANDARD 14)
add_library(cgltf STATIC cgltf.h cgltf.cpp)