# Auth: Alberto Taiuti, Github usr: snowzufer

cmake_minimum_required(VERSION 2.8)

project(lodepng)

add_library(lodepng
  ${CMAKE_CURRENT_SOURCE_DIR}/lodepng.cpp
  ${CMAKE_CURRENT_SOURCE_DIR}/lodepng_util.cpp
  ${CMAKE_CURRENT_SOURCE_DIR}/pngdetail.cpp)

target_include_directories(lodepng PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})

export(TARGETS lodepng FILE lodepng.cmake)

