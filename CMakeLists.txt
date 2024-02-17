cmake_minimum_required(VERSION 3.22)
project(plateformer)

set(CMAKE_CXX_STANDARD 20)

file(GLOB_RECURSE SOURCES "src/*.cpp")

include_directories(include)
add_executable(plateformer ${SOURCES})
target_link_libraries(plateformer sfml-graphics sfml-window sfml-system)
