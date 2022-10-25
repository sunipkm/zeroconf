cmake_minimum_required(VERSION 2.8)
project(zeroconf)

include_directories(./src)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")

set(ZEROCONF_BASIC_DEMO_SOURCE_FILES
    src/zeroconf.hpp
    src/zeroconf-detail.hpp
    src/zeroconf-util.hpp
    samples/basic_demo/main.cpp)

add_executable(basic_demo ${ZEROCONF_BASIC_DEMO_SOURCE_FILES})