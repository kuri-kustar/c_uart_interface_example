cmake_minimum_required(VERSION 2.8.3)
project(mavlink_control)
	
include_directories(
 ./mavlink/include/mavlink/v1.0
)

add_executable(mavlink_control mavlink_control.cpp serial_port.cpp autopilot_interface.cpp)
target_link_libraries(mavlink_control -lpthread)
