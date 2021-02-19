cmake_minimum_required (VERSION 3.5)

project(port-tcp)

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

target_link_libraries(${PROJECT_NAME} ws2_32)

set_target_properties(${PROJECT_NAME} PROPERTIES PREFIX "")
