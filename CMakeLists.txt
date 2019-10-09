cmake_minimum_required(VERSION 3.0)

# Name of the project
project(icalendarlib)

set(SRC_icallib date.cpp icalendar.cpp types.cpp)
	

add_library(icalendarlib SHARED ${SRC_icallib})
add_executable(icalendarlib_test main.cpp)
target_link_libraries(icalendarlib_test icalendarlib)
