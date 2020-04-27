cmake_minimum_required(VERSION 3.8)

add_definitions(-DUNICODE -D_UNICODE)

add_library(common
	STATIC
	Camera.cpp
	Camera.h
	d3dApp.cpp
	d3dApp.h
	d3dUtil.cpp
	d3dUtil.h
	d3dx12.h
	DDSTextureLoader.cpp
	DDSTextureLoader.h
	GameTimer.cpp
	GameTimer.h
	GeometryGenerator.cpp
	GeometryGenerator.h
	MathHelper.cpp
	MathHelper.h
	UploadBuffer.h
)

#add_executable (common_test _Test.cpp)
#target_link_libraries(common_test common)