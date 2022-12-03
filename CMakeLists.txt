cmake_minimum_required(VERSION 3.22)
project("RayTrace")
set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
file(GLOB HEADERS ${PROJECT_SOURCE_DIR}/include/*.h)
file(GLOB SRC ${PROJECT_SOURCE_DIR}/*.cpp)
source_group(head FILES ${HEADERS})
source_group(src FILES ${SRC})
add_executable(RayTrace ${HEADERS} ${SRC})
include_directories(
    ${CMAKE_CURRENT_SOURCE_DIR}/include
)