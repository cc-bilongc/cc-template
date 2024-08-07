add_library(
        cc_main
        OBJECT
        main.cpp
)

set(ALL_OBJECT_FILES
        ${ALL_OBJECT_FILES} $<TARGET_OBJECTS:cc_main>
        PARENT_SCOPE)

set(CC_MAIN_SOURCES main.cpp)

add_executable(ccwc ${CC_MAIN_SOURCES})
