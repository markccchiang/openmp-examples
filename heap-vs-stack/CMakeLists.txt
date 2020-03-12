cmake_minimum_required(VERSION 3.6)

set(LINK_LIBS ${LINK_LIBS} ${OpenMP_CXX_LIBRARIES})
set(SOURCE_FILES ${SOURCE_FILES} main.cpp)

add_executable(heap_vs_stack ${SOURCE_FILES})
target_link_libraries(heap_vs_stack ${LINK_LIBS})
