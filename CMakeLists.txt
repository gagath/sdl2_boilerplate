cmake_minimum_required(VERSION 2.8)

project(sdl2_boilerplate)

set(
    CMAKE_MODULE_PATH
    $(CMAKE_MODULE_PATH)
    "${CMAKE_SOURCE_DIR}/cmake/"
)

set(
    EXECUTABLE_NAME
    "test"
)

find_package(SDL2 REQUIRED)
find_package(SDL2_image REQUIRED)
find_package(SDL2_ttf REQUIRED)
find_package(SDL2_mixer REQUIRED)

include_directories(
    ${SDL2_INCLUDE_DIR}
    ${SDL2_IMAGE_INCLUDE_DIR}
)

add_executable(
    ${EXECUTABLE_NAME}
    src/main.c
)

target_link_libraries(
    ${EXECUTABLE_NAME}
    ${SDL2_LIBRARY}
    ${SDL2_IMAGE_LIBRARY}
    ${SDL2_TTF_LIBRARY}
    ${SDL2_MIXER_LIBRARY}
)
