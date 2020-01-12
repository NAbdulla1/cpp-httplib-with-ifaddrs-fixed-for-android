cmake_minimum_required(VERSION 3.7.0)

project(ifaddrslib)

set(CMAKE_CXX_STANDARD 11)

# Include
include(GNUInstallDirs)
include(ExternalProject)

set(IF_ADDR_LIB ${PROJECT_NAME})

add_library(${IF_ADDR_LIB} SHARED ifaddrs.c)
target_include_directories(${IF_ADDR_LIB} PUBLIC ./include)