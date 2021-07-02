cmake_minimum_required(VERSION 2.8)
project( tracking )
find_package( OpenCV REQUIRED )
include_directories( ${OpenCV_INCLUDE_DIRS} )

file(GLOB SOURCES src/*.?pp)
add_executable(${PROJECT_NAME} ${SOURCES})

target_link_libraries( ${PROJECT_NAME}  ${OpenCV_LIBS} )

