cmake_minimum_required(VERSION 3.16 FATAL_ERROR)

project(Sorse)

# set some global properties
set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set_property(GLOBAL PROPERTY USE_FOLDERS ON)

# add the subdirectories
add_subdirectory(${PROJECT_SOURCE_DIR}/Engine)
add_subdirectory(${PROJECT_SOURCE_DIR}/Sandbox)