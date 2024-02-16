cmake_minimum_required(VERSION 3.5)

project(2D_Racing)

set(CMAKE_CXX_STANDARD 11)

# Add the include directory for ThirdParty
include_directories(${CMAKE_SOURCE_DIR}/ThirdParty)

add_executable(${PROJECT_NAME} src/RetroRacer.cpp)

target_link_libraries(${PROJECT_NAME} PRIVATE User32.lib)