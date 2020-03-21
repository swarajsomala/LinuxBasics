message(Name ,${PROJECT_NAME})

include(GNUInstallDirs)

add_library(${PROJECT_NAME} SHARED  hello.cpp)

target_include_directories(${PROJECT_NAME} PUBLIC
    $<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}/../inc>
    $<INSTALL_INTERFACE:include>
    )

# set_target_properties(${PROJECT_NAME} PROPERTIES
# OUTPUT_NAME cml_${PROJECT_NAME}
# )

