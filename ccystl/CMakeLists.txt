cmake_minimum_required(VERSION 3.29)
project(ccystl)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

link_directories(${LIB_DIR})
set(ADAPTER_DIR ${MAIN_PROJECT_DIR}/adapter)
set(ALGORITHM_DIR ${MAIN_PROJECT_DIR}/algorithm)
set(ALLOCATOR_DIR ${MAIN_PROJECT_DIR}/allocator)
set(CONTAINER_DIR ${MAIN_PROJECT_DIR}/container)
set(FUNCTOR_DIR ${MAIN_PROJECT_DIR}/functor)
set(ITERATOR_DIR ${MAIN_PROJECT_DIR}/iterator)
set(UTILS_DIR ${MAIN_PROJECT_DIR}/utils)

add_subdirectory(${ADAPTER_DIR})
add_subdirectory(${ALGORITHM_DIR})
add_subdirectory(${ALLOCATOR_DIR})
add_subdirectory(${CONTAINER_DIR})
add_subdirectory(${FUNCTOR_DIR})
add_subdirectory(${ITERATOR_DIR})
add_subdirectory(${UTILS_DIR})