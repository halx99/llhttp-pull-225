cmake_minimum_required(VERSION 3.24)
project(test)

set(CMAKE_CXX_STANDARD 17)

include(cmake/CPM.cmake)

message(STATUS "Hello world(2)")

CPMAddPackage(
  NAME dummy-3rds
  VERSION main
  GITHUB_REPOSITORY halx99/dummy-3rds
  GIT_TAG "main"
)

add_executable(test main.cpp)
target_link_libraries(test dummy-3rds)
