cmake_minimum_required(VERSION 3.1)

# Project
project(HelloWorldEmoticons)
find_package(Qt5Widgets CONFIG REQUIRED)

# Options
set(CMAKE_AUTOMOC ON)
set(CMAKE_AUTORCC ON)
set(CMAKE_AUTOUIC ON)
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

# Application
add_executable(HelloWorldEmoticons WIN32 MACOSX_BUNDLE src/HelloWorldEmoticons.cpp src/HelloWorldEmoticons.h)
target_link_libraries(HelloWorldEmoticons Qt5::Widgets)
