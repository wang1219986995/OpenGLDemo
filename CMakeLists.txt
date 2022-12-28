cmake_minimum_required(VERSION 3.23)
project(OpenGLDemo)

set(CMAKE_CXX_STANDARD 17)


include_directories(${PROJECT_SOURCE_DIR}/include/)

link_directories(${PROJECT_SOURCE_DIR}/lib/)

add_executable(OpenGLDemo
        main.cpp
        glad.c)

target_link_libraries(OpenGLDemo
        glfw3)