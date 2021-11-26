cmake_minimum_required(VERSION 3.0.0)
project(CreateC++Project VERSION 0.1.0)

include(CTest)
enable_testing()

add_compile_options(-fstandalone-debug)
add_executable(CreateC++Project main.cpp)

# 自动导出complie——commands.json
set(CMAKE_EXPORT_COMPILE_COMMANDS ON)
set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)
