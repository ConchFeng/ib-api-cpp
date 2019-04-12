set(PROJECT_NAME TestCppClient)

file(GLOB TestCppClient-header "*.h")
file(GLOB TestCppClient-source "*.cpp")

include_directories("../")
include_directories("../client")

add_executable(${PROJECT_NAME} ${TestCppClient-header} ${TestCppClient-source})

target_link_libraries(${PROJECT_NAME} client-lib)