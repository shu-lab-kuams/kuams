cmake_minimum_required(VERSION 3.8)
project(kuams)

if(CMAKE_COMPILER_IS_GNUCXX OR CMAKE_CXX_COMPILER_ID MATCHES "Clang")
  add_compile_options(-Wall -Wextra -Wpedantic)
endif()

add_subdirectory(kuams_navigation)
add_subdirectory(kuams_bringup)
add_subdirectory(kuams_description)
add_subdirectory(kuams_slam)
