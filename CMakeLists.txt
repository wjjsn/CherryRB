cmake_minimum_required(VERSION 3.22)
enable_language(C CXX)

add_library(CherryRB OBJECT)
target_sources(CherryRB PRIVATE "${CMAKE_CURRENT_LIST_DIR}/chry_ringbuffer.c")
target_include_directories(CherryRB PUBLIC "${CMAKE_CURRENT_LIST_DIR}")

# 使用方式（消费方）: target_link_libraries(<你的目标> PRIVATE CherryRB)