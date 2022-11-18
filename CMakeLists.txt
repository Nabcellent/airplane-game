cmake_minimum_required(VERSION 3.23)
project(CAT2)

set(CMAKE_CXX_STANDARD 14)

find_package(OpenGL REQUIRED)
find_package(GLUT REQUIRED)

include_directories(${OPENGL_INCLUDE_DIRS} ${GLUT_INCLUDE_DIRS})

add_executable(CAT2 main.cpp)
#add_executable(CAT2 tree.cpp)

target_link_libraries(CAT2 glfw ${OPENGL_LIBRARIES} ${GLUT_LIBRARY})
