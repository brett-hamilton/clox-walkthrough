cmake_minimum_required(VERSION 3.28)

project(Clox LANGUAGES C)

add_executable(clox)

target_sources(clox
  PRIVATE
    main.c
    chunk.c
    memory.c
    debug.c
)

target_include_directories(clox
  PUBLIC
    ${CMAKE_CURRENT_SOURCE_DIR}/include
)
