## gflags package configuration tests

cmake_minimum_required (VERSION 3.5 FATAL_ERROR)

project (gflags_${TEST_NAME})

find_package (gflags REQUIRED)

add_executable (foo main.cc)
target_link_libraries (foo gflags::gflags)
