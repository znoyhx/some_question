cmake_minimum_required(VERSION 3.10)

project(IDontCare VERSION 1.0)

aux_source_directory(${CMAKE_CURRENT_SOURCE_DIR}/src SRC_LIST)

include_directories(${CMAKE_CURRENT_SOURCE_DIR}/inc)

add_library(myFunction SHARED ${SRC_LIST})

set_target_properties(myFunction PROPERTIES
    LIBRARY_OUTPUT_DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}/lib
)





