cmake_minimum_required(VERSION 2.8)
project( Viewsynthesis )
find_package( OpenCV REQUIRED )

set(SRC_FILES
    ./filter.cpp
    ./guidedFilter.cpp
    ./main.cpp
    ./util.cpp
    ./ViewSynthesis.cpp
)

add_executable( Viewsynthesis ${SRC_FILES} )
target_link_libraries( Viewsynthesis ${OpenCV_LIBS} )
