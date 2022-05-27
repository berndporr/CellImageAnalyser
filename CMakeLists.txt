cmake_minimum_required(VERSION 3.1)
project( CellImageAnalyser LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 11)

if(NOT CMAKE_BUILD_TYPE AND NOT CMAKE_CONFIGURATION_TYPES)
  set(CMAKE_BUILD_TYPE "RelWithDebInfo")
endif()

cmake_policy(SET CMP0048 NEW) # set VERSION in project()
cmake_policy(SET CMP0042 NEW) # enable MACOSX_RPATH by default

include(GNUInstallDirs)

find_package( OpenCV REQUIRED )
add_executable( ellipse ellipse.cpp )
target_link_libraries( ellipse ${OpenCV_LIBS} )


