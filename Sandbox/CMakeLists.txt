project(Sandbox)

add_executable(Sandbox ${PROJECT_SOURCE_DIR}/src/main.cpp)

target_link_libraries(Sandbox PUBLIC Engine)