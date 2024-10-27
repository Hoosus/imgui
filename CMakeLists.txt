cmake_minimum_required(VERSION 3.0)
project(ImGui)

set(IMGUI_SOURCES
    imgui.cpp
    imgui_draw.cpp
    imgui_widgets.cpp
    imgui_tables.cpp
)

set(IMGUI_SPECIFIC_SOURCES
)

add_library(imgui STATIC ${IMGUI_SOURCES})
target_include_directories(imgui PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})