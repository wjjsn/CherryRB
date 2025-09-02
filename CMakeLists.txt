cmake_minimum_required(VERSION 3.22)
enable_language(C)

add_library(CherryRB OBJECT)
target_sources(CherryRB PRIVATE chry_ringbuffer.c)
target_include_directories(CherryRB PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})
target_link_libraries(${CMAKE_PROJECT_NAME} PRIVATE CherryRB)