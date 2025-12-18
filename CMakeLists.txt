cmake_minimum_required(VERSION 3.16)
project(3Civ LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

set(SFML_DIR "${CMAKE_SOURCE_DIR}/external/SFML-2.6.2/lib/cmake/SFML")

find_package(SFML 2.6 COMPONENTS system window graphics audio REQUIRED)

file(GLOB_RECURSE SOURCES
    src/*.cpp
)

add_executable(3Civ ${SOURCES})

target_include_directories(3Civ PRIVATE include)

target_link_libraries(3Civ
    sfml-system
    sfml-window
    sfml-graphics
    sfml-audio
)

add_custom_command(TARGET 3Civ POST_BUILD
    COMMAND ${CMAKE_COMMAND} -E copy_directory
    "${CMAKE_SOURCE_DIR}/external/SFML-2.6.2/bin"
    $<TARGET_FILE_DIR:3Civ>)