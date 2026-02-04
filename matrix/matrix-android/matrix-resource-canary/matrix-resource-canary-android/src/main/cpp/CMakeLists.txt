cmake_minimum_required(VERSION 3.10.2)
# 16KB page size alignment for Android
add_link_options(-Wl,-z,max-page-size=16384 -Wl,-z,common-page-size=16384)
project(matrix-resource-canary-android)

set(CMAKE_CXX_STANDARD 17)

add_subdirectory(memory_util)