cmake_minimum_required (VERSION 3.5)

project(port-serial)

add_library(${PROJECT_NAME} SHARED
    comio.cpp
    comio.h
    comparams.cpp
    comparams.h
    comport.cpp
    comport.h
    import.h
    port.cpp
    precomp.cpp
    precomp.h
    ../plugins.def
)

set_target_properties(${PROJECT_NAME} PROPERTIES PREFIX "")
