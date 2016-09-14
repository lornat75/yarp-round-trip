cmake_minimum_required(VERSION 2.8)

project(latency)

find_package(YARP REQUIRED)

include_directories(${YARP_INCLUDE_DIRS})

add_executable(latency port_latency_st.cpp)

target_link_libraries(latency ${YARP_LIBRARIES})