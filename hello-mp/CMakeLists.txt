cmake_minimum_required(VERSION 3.6)

set(LINK_LIBS ${LINK_LIBS} ${OpenMP_CXX_LIBRARIES})
set(SOURCE_FILES ${SOURCE_FILES} main.cpp)

add_executable(hello_mp ${SOURCE_FILES})
target_link_libraries(hello_mp ${LINK_LIBS})
