cmake_minimum_required (VERSION 3.5)

project(filter-telnet)

add_library(${PROJECT_NAME} SHARED
    filter.cpp
    import.h
    opt_comport.cpp
    opt_comport.h
    opt_termtype.cpp
    opt_termtype.h
    precomp.cpp
    precomp.h
    telnet.cpp
    telnet.h
    ../plugins.def
)

set_target_properties(${PROJECT_NAME} PROPERTIES PREFIX "")
