cmake_minimum_required(VERSION 3.16)
project(test_framework)

# Create library
add_library(test_framework STATIC)
target_sources(test_framework PRIVATE
        test_framework/test_framework.hpp
        src/test_framework.cpp
        test_framework/test_framework.h
        src/test_framework.c
        )
target_include_directories(test_framework PUBLIC test_framework)
