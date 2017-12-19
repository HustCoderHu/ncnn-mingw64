project(aaaa)
cmake_minimum_required(VERSION 3.10)


set(OpenCV_DIR "E:/Libs/opencv-3.3.1/build/install")
find_package(OpenCV QUIET COMPONENTS core highgui imgproc imgcodecs)
if(NOT OpenCV_FOUND)
    find_package(OpenCV REQUIRED COMPONENTS core highgui imgproc)
endif()

message("OpenCV_VERSION: " ${OpenCV_VERSION})
message("OpenCV_INCLUDE_DIRS: " ${OpenCV_INCLUDE_DIRS})
message("OpenCV_LIBS: " ${OpenCV_LIBS})

