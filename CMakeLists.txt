cmake_minimum_required(VERSION 3.16)
project(CMakeProject LANGUAGES CXX)

# --- CMAKE-SPECIFIC CONFIGURATION ---
set(FETCHCONTENT_QUIET FALSE)
set(CMAKE_EXPORT_COMPILE_COMMANDS ON)
set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

# --- PROJECT-WIDE OPTIONS ---
set(BINARY ${CMAKE_PROJECT_NAME})

# --- PROJECT CONFIGURATION ---
add_subdirectory(src)