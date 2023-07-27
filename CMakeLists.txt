project(MOYFClient)
cmake_minimum_required(VERSION 3.19)

add_subdirectory(MOYFNetworking)
link_libraries(ws2_32)
link_libraries(wsock32)

add_subdirectory(MOYFClient)
add_subdirectory(MOYFServer)