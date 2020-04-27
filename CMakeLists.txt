# CMakeList.txt : Top-level CMake project file, do global configuration
# and include sub-projects here.
#
cmake_minimum_required (VERSION 3.8)

project ("VDX12_CMake")


#UNICODE to process file
add_definitions(-DUNICODE -D_UNICODE)

#first we add the Common Libraries
add_subdirectory("Common")

#Set the Header and libraries files for our project
include_directories(${VDX12_CMake_SOURCE_DIR}/Common)
link_directories(${VDX12_CMake_SOURCE_DIR}/Common)

# Include sub-projects.
add_subdirectory ("C1_VectorAlgebra")

add_subdirectory("C2_MatrixAlgebra")


add_subdirectory("C4_Init")
