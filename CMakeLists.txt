cmake_minimum_required(VERSION 3.16)
project(testing_framework)

# Create library
add_library(testing_framework STATIC)
target_sources(testing_framework PRIVATE
        test_framework/test_framework.hpp
        src/test_framework.cpp
        test_framework/test_framework.h
        src/test_framework.c
        )
target_include_directories(testing_framework PUBLIC test_framework)
