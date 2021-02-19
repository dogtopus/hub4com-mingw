cmake_minimum_required (VERSION 3.5)

project(port-connector)

add_library(${PROJECT_NAME} SHARED
    comport.cpp
    comport.h
    import.h
    port.cpp
    precomp.cpp
    precomp.h
    ../plugins.def
)

set_target_properties(${PROJECT_NAME} PROPERTIES PREFIX "")
