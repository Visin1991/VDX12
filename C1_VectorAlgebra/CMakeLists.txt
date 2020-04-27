# CMakeList.txt : CMake project for VDX12_CMake, include source and define
# project specific logic here.
#
cmake_minimum_required (VERSION 3.8)


add_executable (VectorAlgebra xmvec3.cpp)
target_link_libraries(VectorAlgebra common)

# TODO: Add tests and install targets if needed.
