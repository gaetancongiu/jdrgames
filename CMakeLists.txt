cmake_minimum_required(VERSION 3.10)
project(jdrgames)

set(CMAKE_CXX_STANDARD 14)

include(${CMAKE_BINARY_DIR}/conanbuildinfo.cmake)
conan_basic_setup()

add_executable(jdrgames main.cpp Personnage.cpp Personnage.h)
target_link_libraries(jdrgames ${CONAN_LIBS})