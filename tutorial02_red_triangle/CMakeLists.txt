set(TARGET_NAME tutorial02_red_triangle)
add_executable(${TARGET_NAME} tutorial02.cpp)

target_link_libraries(${TARGET_NAME} PRIVATE
    glfw
    GLEW::GLEW
    opengl32.lib
    )

set_target_properties(${TARGET_NAME} PROPERTIES
    VS_DEBUGGER_WORKING_DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}
    )
