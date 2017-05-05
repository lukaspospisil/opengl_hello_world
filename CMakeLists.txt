project(OPENGL_HELLO_WORLD)
cmake_minimum_required(VERSION 2.8)

add_executable(hello_world hello_world.cpp)
find_package(OpenGL REQUIRED)
find_package(GLUT REQUIRED)
include_directories( ${OPENGL_INCLUDE_DIRS}  ${GLUT_INCLUDE_DIRS} )

target_link_libraries(hello_world ${OPENGL_LIBRARIES} ${GLUT_LIBRARY} )


