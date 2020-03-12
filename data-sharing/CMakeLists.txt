cmake_minimum_required(VERSION 3.6)

set(LINK_LIBS ${LINK_LIBS} ${OpenMP_CXX_LIBRARIES})
set(SOURCE_FILES ${SOURCE_FILES} main.cpp)

add_executable(data_sharing ${SOURCE_FILES})
target_link_libraries(data_sharing ${LINK_LIBS})
