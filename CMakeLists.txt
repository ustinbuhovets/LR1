cmake_minimum_required(VERSION 3.25)
project(Lab1 LANGUAGES CXX)

set(CMAKE_CXX_STANDART 23)
set(CMAKE_CXX_STANDART_REQUIRED ON)

include(FetchContent)
FetchContent_Declare(
    fmt
    GIT_REPOSITORY https://github.com/fmtlib/fmt.git
    GIT_TAG 11.0.0 
)

FetchContent_MakeAvailable(fmt)


add_executable(Lab1 Type_3.cpp)
target_link_libraries(Lab1 PRIVATE fmt::fmt)
