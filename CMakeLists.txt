cmake_minimum_required(VERSION 3.5 FATAL_ERROR)
project(mimic VERSION 0.0.1 LANGUAGES CXX)

include_directories(include)

set(gtest_force_shared_crt ON CACHE BOOL "" FORCE)
add_subdirectory(googletest)

add_subdirectory(common)