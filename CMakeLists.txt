cmake_minimum_required (VERSION 2.8.11)
project (nanomsg-examples)

set(CMAKE_MODULE_PATH "${CMAKE_CURRENT_SOURCE_DIR}/cmake")

find_package(PkgConfig)
pkg_search_module(libnanomsg REQUIRED libnanomsg)

include_directories(${libnanomsg_INCLUDEDIR})

add_definitions(-Wall -Wextra -Werror)

add_subdirectory(c)
add_subdirectory(cpp)
