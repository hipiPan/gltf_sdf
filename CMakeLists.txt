cmake_minimum_required(VERSION 3.13)
project(gltf_sdf)
set(CMAKE_CXX_STANDARD 14)

add_library(gltf_sdf STATIC gltf_sdf.h gltf_sdf.cpp)
target_include_directories(gltf_sdf PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})

add_subdirectory(extern/cgltf)
target_link_libraries(gltf_sdf PUBLIC cgltf)