cmake_minimum_required(version 3.10)
project(OpenGLApp)

find_package(OpenGL REQUIRED)

find_package(glfw3 REQUIRED)

include_directories(E:\Proprietary\Game_Engines\PL3DGE)

add_executable(OpenGLApp src/main.cpp src/glad.c)

target_link_libraries(OpenGLApp PRIVATE OpenGL:GL glfw)