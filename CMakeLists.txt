cmake_minimum_required(VERSION 3.17)
project(OpenGLTemplate)

set(CMAKE_CXX_STANDARD 17)

add_executable(OpenGLTemplate main.cpp)

find_package(glfw3 3.3 REQUIRED)
target_link_libraries(OpenGLTemplate glfw)
find_package(OpenGL REQUIRED)
target_link_libraries(OpenGLTemplate OpenGL::GL)
find_package(GLEW 2.2 REQUIRED)
target_link_libraries(OpenGLTemplate GLEW::GLEW)