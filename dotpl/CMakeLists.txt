cmake_minimum_required (VERSION 3.8)


set(CMAKE_OSX_DEPLOYMENT_TARGET "10.14")

project(dotpl)

file(GLOB_RECURSE SOURCES "source/*.cpp")
file(GLOB_RECURSE HEADERS "source/*.hpp")

add_executable(dotpl ${SOURCES} ${HEADERS})

set_target_properties(dotpl PROPERTIES
        CXX_STANDARD 17
        CXX_STANDARD_REQUIRED OFF
        CXX_EXTENSIONS OFF
        )
