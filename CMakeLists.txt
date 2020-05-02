cmake_minimum_required(VERSION 3.1)

project(cpp_base64)

add_library(${PROJECT_NAME} base64.cpp)
set_target_properties(${PROJECT_NAME} PROPERTIES PUBLIC_HEADER base64.h)

include(GNUInstallDirs)
install(TARGETS ${PROJECT_NAME})
