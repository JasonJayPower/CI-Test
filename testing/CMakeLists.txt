#Require a minimum version of cmake.
cmake_minimum_required(VERSION 3.15)

#Set the name of the project.
project(Testing
    VERSION 1.0
    DESCRIPTION "Testing"
    LANGUAGES CXX)
  
# File manipulation command. (Automatically checks and finds all source files at build time)
file(GLOB_RECURSE SRC_FILES CONFIGURE_DEPENDS "src/*.cpp")

# Add an executable to the project using the specified source files.
add_executable(${PROJECT_NAME} ${SRC_FILES})

# Add include directories to a target.
target_include_directories(${PROJECT_NAME} PUBLIC ${PROJECT_SOURCE_DIR}/src)
