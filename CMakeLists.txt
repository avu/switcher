cmake_minimum_required(VERSION 3.24)
project(switcher)

set(CMAKE_CXX_STANDARD 14)
FIND_LIBRARY(APPKIT_LIBRARY AppKit)

add_executable(switcher main.mm)
target_link_libraries(switcher "-framework Cocoa")
target_link_libraries(switcher "-framework IOKit")
