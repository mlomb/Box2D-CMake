cmake_minimum_required(VERSION 2.6)

project(Box2D)

file(GLOB_RECURSE Box2D_SRC
	Box2D/Box2D/*.h
	Box2D/Box2D/*.cpp
)

include_directories(Box2D/Box2D)

add_library(Box2D STATIC ${Box2D_SRC})