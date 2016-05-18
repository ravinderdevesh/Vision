cmake_minimum_required(VERSION 2.8)
    project( vis )
    set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${vis_SOURCE_DIR}/build)
    find_package( OpenCV REQUIRED )
    add_executable( vis 
                    flann.cpp 

                  )
    target_link_libraries(vis  ${OpenCV_LIBS} )
