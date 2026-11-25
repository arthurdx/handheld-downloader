cmake_minimum_required(VERSION 3.16)
project(handheld-dl CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
if(NOT CMAKE_BUILD_TYPE)
  set(CMAKE_BUILD_TYPE Release)
endif()

find_package(SDL2 REQUIRED)

add_executable(handheld-dl src/main.cpp)
target_include_directories(handheld-dl PRIVATE ${SDL2_INCLUDE_DIRS})
target_link_libraries(handheld-dl PRIVATE ${SDL2_LIBRARIES})
target_compile_options(handheld-dl PRIVATE -Wall -Wextra -Wpedantic)
