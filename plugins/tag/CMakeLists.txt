cmake_minimum_required (VERSION 3.5)

project(filter-tag)

add_library(${PROJECT_NAME} SHARED
    filter.cpp
    precomp.cpp
    precomp.h
    ../plugins.def
)

set_target_properties(${PROJECT_NAME} PROPERTIES PREFIX "")
