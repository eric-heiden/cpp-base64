cmake_minimum_required(VERSION 3.1)

project(cpp_base64)

add_library(cpp_base64 base64.cpp)
set_target_properties(cpp_base64 PROPERTIES PUBLIC_HEADER base64.h)

include(GNUInstallDirs)
install(TARGETS cpp_base64 DESTINATION ${CMAKE_INSTALL_INCLUDEDIR}/${PROJECT_NAME})
