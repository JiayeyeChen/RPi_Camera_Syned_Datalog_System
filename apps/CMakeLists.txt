cmake_minimum_required(VERSION 3.6)

project(libcamera-vid-mine)
add_executable(libcamera-vid-mine libcamera_vid_mine.cpp)
target_link_libraries(libcamera-vid-mine libcamera_app encoders outputs)


set(EXECUTABLES libcamera-vid-mine)


set(EXECUTABLE_OUTPUT_PATH  ${CMAKE_BINARY_DIR})
install(TARGETS ${EXECUTABLES} RUNTIME DESTINATION bin)
