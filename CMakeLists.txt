cmake_minimum_required(VERSION 3.3)

project(boost_optional)

add_library(boost_optional INTERFACE)

target_include_directories(boost_optional BEFORE INTERFACE ${CMAKE_CURRENT_SOURCE_DIR}/include)

install(TARGETS boost_optional DESTINATION lib)
install(DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}/include/boost DESTINATION include)
