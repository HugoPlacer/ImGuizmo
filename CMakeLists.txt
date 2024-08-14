project(ImGuizmo VERSION 0.1.0 LANGUAGES C CXX)

set(SOURCES
        "${CMAKE_CURRENT_SOURCE_DIR}/ImGuizmo.h"
        "${CMAKE_CURRENT_SOURCE_DIR}/ImGuizmo.cpp")

add_library(${PROJECT_NAME} STATIC ${SOURCES})

target_include_directories(${PROJECT_NAME}
    PUBLIC "${CMAKE_CURRENT_SOURCE_DIR}"
)

target_link_libraries(${PROJECT_NAME} ImGui)
