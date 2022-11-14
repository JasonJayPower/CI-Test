#Require a minimum version of cmake.
cmake_minimum_required(VERSION 3.15)

#Set the name of the project.
project(CI-Test
    VERSION 1.0
    DESCRIPTION "CI-Test"
    LANGUAGES CXX)

message(PROJECT_SOURCE_DIR="${CMAKE_SOURCE_DIR}")

add_subdirectory(game)
add_subdirectory(testing)