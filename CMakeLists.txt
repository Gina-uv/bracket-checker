cmake_minimum_required(VERSION 3.16)
project(bracket_checker LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

add_compile_options(-Wall -Wextra)

add_executable(bracket_checker
    src/main.cpp
    src/match.cpp
    src/error_format.cpp
    src/cli_ui.cpp
    src/file_checker.cpp
    src/task_queue.cpp
)

target_include_directories(bracket_checker PRIVATE include)