cmake_minimum_required(VERSION 3.16)
project(NewOpenGL)

set(CMAKE_CXX_STANDARD 14)

include_directories(Dependencies/GLEW/include)
include_directories(Dependencies/GLEW/include/GL)
include_directories(Dependencies/GLFW/include)
include_directories(Dependencies/GLFW/include/GLFW)
include_directories(NewOpenGL/src)

add_executable(NewOpenGL
        Dependencies/GLEW/include/GL/eglew.h
        Dependencies/GLEW/include/GL/glew.h
        Dependencies/GLEW/include/GL/glxew.h
        Dependencies/GLEW/include/GL/wglew.h
        Dependencies/GLFW/include/GLFW/glfw3.h
        Dependencies/GLFW/include/GLFW/glfw3native.h
        NewOpenGL/res/shaders/basic.shader
        NewOpenGL/src/Application.cpp
        NewOpenGL/src/IndexBuffer.cpp
        NewOpenGL/src/IndexBuffer.h
        NewOpenGL/src/Renderer.cpp
        NewOpenGL/src/Renderer.h
        NewOpenGL/src/Shader.cpp
        NewOpenGL/src/Shader.h
        NewOpenGL/src/VertexArray.cpp
        NewOpenGL/src/VertexArray.h
        NewOpenGL/src/VertexBuffer.cpp
        NewOpenGL/src/VertexBuffer.h
        NewOpenGL/src/VertexBufferLayout.h)
