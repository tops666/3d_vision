cmake_minimum_required(VERSION 3.1)
project(try_lightfilter)
add_definitions(--std=c++11 -Wno-unknown-pragmas)

find_package(catkin_simple REQUIRED)
catkin_simple(ALL_DEPS_REQUIRED)

cs_add_executable(${PROJECT_NAME}
    src/main.cc
)

cs_install()
cs_export()

