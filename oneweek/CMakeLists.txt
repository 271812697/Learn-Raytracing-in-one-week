file(GLOB HEADERS ${CMAKE_CURRENT_SOURCE_DIR}/*.h)
file(GLOB SRC ${CMAKE_CURRENT_SOURCE_DIR}/*.cpp)
source_group(head FILES ${HEADERS})
source_group(src FILES ${SRC})
add_executable(RayTrace ${HEADERS} ${SRC})

