cmake_minimum_required(VERSION 3.18.4)

project(rogue_test)

add_executable(${PROJECT_NAME} main.c)

find_package(libtcod)

target_link_libraries(${PROJECT_NAME} PRIVATE ${LIBTCOD_LIBRARY})