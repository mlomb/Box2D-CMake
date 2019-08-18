cmake_minimum_required(VERSION 3.0)

project(Box2D)

file(GLOB_RECURSE Box2D_SRC
	Box2D/Box2D/*.h
	Box2D/Box2D/*.cpp
)

add_library(Box2D STATIC ${Box2D_SRC})

target_include_directories(Box2D PUBLIC "Box2D")
