project(Engine)

include(Sources.cmake)

add_library(Engine STATIC ${SOURCES})

# add external libraries
add_Subdirectory(${PROJECT_SOURCE_DIR}/external/spdlog)

# add headers
target_include_directories(Engine PUBLIC ${PROJECT_SOURCE_DIR}/src)
target_include_directories(Engine PUBLIC ${PROJECT_SOURCE_DIR}/external/spdlog/include)

# link against external libraries
target_link_libraries(Engine PUBLIC spdlog::spdlog)
