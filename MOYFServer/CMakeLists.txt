cmake_minimum_required(VERSION 3.19)
project(MOYFServer)
link_libraries(ws2_32)
link_libraries(wsock32)

set(CMAKE_CXX_STANDARD 20)

add_executable(${PROJECT_NAME} main.cpp)

target_include_directories(${PROJECT_NAME}
        PUBLIC
            MOYFNetworking
)

target_link_libraries(${PROJECT_NAME}
        PUBLIC
            MOYFNetworking
)