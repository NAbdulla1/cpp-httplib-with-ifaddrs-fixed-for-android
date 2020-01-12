cmake_minimum_required(VERSION 3.7.0)

project(httplib)

set(CMAKE_CXX_STANDARD 11)

# Include
include(GNUInstallDirs)
include(ExternalProject)

set(CPP_HTTP_LIB ${PROJECT_NAME})

add_library(${CPP_HTTP_LIB} SHARED httplib.cc)

target_include_directories(${CPP_HTTP_LIB} PUBLIC ${CMAKE_SOURCE_DIR}/include)

#add_subdirectory(example)
#add_subdirectory(test)

add_subdirectory(android-ifaddrs)
target_link_libraries(${CPP_HTTP_LIB} ${IF_ADDR_LIB})