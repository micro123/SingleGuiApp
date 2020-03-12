cmake_minimum_required(VERSION 3.10 FATAL_ERROR)

project(SingleGui CXX C)

option(PACKAGE_TESTS "Build the tests" ON)
if(PACKAGE_TESTS)
    enable_testing()
    include(GoogleTest)
    add_subdirectory(tests)
endif()
