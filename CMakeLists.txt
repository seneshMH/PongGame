cmake_minimum_required(VERSION 3.22.2)

project(Pong)

set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_SOURCE_DIR}/bin)
add_executable(${PROJECT_NAME} main.cpp)

add_subdirectory(external/raylib)
target_link_libraries(${PROJECT_NAME} raylib opengl32 gdi32 winmm)
