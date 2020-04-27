cmake_minimum_required(VERSION 3.8)


add_executable(Init WIN32 InitDirect3DApp.cpp)
target_link_libraries(Init common)