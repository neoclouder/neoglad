cmake_minimum_required(VERSION 3.25)
project(neoglad LANGUAGES C)

set(NEOGLAD_NAME neoglad)
add_library(${NEOGLAD_NAME} INTERFACE)

target_include_directories(${NEOGLAD_NAME} INTERFACE
  $<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}/include>
)
