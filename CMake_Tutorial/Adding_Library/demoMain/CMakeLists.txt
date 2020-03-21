set(execlib "cmake-lib-demo")
add_executable(${execlib} Demo.cpp)

target_link_libraries(${execlib} ${PROJECT_NAME})

