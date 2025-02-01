cmake_minimum_required(VERSION 3.24)
set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

set(target DearWidgets)
project(${target} LANGUAGES CXX)

set(SRCS
  src/api/dear_widgets.h
  src/api/dear_widgets.cpp
)

add_library(${target} ${SRCS})

target_include_directories(${target} PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}/src/api)
