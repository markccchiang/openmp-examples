cmake_minimum_required(VERSION 3.6)
project(openmp_examples)

set(CMAKE_CXX_STANDARD 14)

# Enable OpenMP if package is found
find_package(OpenMP)
if (OPENMP_FOUND)
    set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} ${OpenMP_C_FLAGS}")
    set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} ${OpenMP_CXX_FLAGS}")
else ()
    message(WARNING "OpenMP not found!")
endif ()

add_subdirectory(hello-mp)
add_subdirectory(avrage-reduction)
add_subdirectory(data-sharing)
add_subdirectory(heap-vs-stack)
add_subdirectory(integral)
add_subdirectory(linkedlist)
add_subdirectory(Matrix)
add_subdirectory(parallel-loop-1)
add_subdirectory(scheduling)
