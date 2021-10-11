cmake_minimum_required(VERSION 3.18)
project(hello_boost VERSION 0.0.1)

find_package(Boost 1.71 REQUIRED COMPONENTS program_options)
add_executable(hello_boost hello_boost.cpp )
target_link_libraries(hello_boost Boost::program_options)
