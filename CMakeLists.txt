cmake_minimum_required (VERSION 3.5)

project(hub4com)

add_executable(${PROJECT_NAME}
    comhub.cpp
    export.cpp
    filters.cpp
    hub4com.cpp
    hubmsg.cpp
    plugins.cpp
    port.cpp
    precomp.cpp
    route.cpp
    static.cpp
    timer.cpp
    utils.cpp
    hub4com.rc
)

add_subdirectory(plugins)
