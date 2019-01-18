cmake_minimum_required(VERSION 3.1)

project(gamejam_base)

set (SFML_STATIC_LIBRARIES TRUE)
find_package(SFML 2.5 COMPONENTS graphics REQUIRED)

set (SOURCES
	src/main.cpp
)

add_executable(game ${SOURCES})

target_link_libraries(game sfml-graphics)