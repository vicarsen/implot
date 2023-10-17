cmake_minimum_required(VERSION 3.10)
set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED TRUE)

project(ImPlot)

add_library(${PROJECT_NAME}
    ./implot.cpp
    ./implot_demo.cpp
    ./implot_items.cpp
)

target_link_libraries(${PROJECT_NAME} PUBLIC
    ImGui
)

target_include_directories(${PROJECT_NAME} PUBLIC
    ./
)

