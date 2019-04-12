cmake_minimum_required(VERSION 3.12)

project(ib-api)

set(CMAKE_CXX_STANDARD 14)
set(CMAKE_CXX_FLAGS "-pthread -Wall -Wno-switch -Wpedantic")

add_subdirectory(client)

add_subdirectory(TestCppClient)