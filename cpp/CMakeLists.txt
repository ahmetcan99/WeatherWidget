cmake_minimum_required(VERSION 3.16)
project(WeatherWidget)

# Find Qt and link the Widgets module
set(CMAKE_AUTOMOC ON)
find_package(Qt5 COMPONENTS Widgets REQUIRED)

add_executable(weatherwidget
    src/widget.cpp
)

target_link_libraries(weatherwidget Qt5::Widgets)