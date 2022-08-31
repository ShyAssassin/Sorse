project(Engine)

include(Sources.cmake)

add_library(Engine STATIC ${SOURCES})

target_include_directories(Engine PUBLIC ${PROJECT_SOURCE_DIR}/src)