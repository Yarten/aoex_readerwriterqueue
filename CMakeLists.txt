cmake_minimum_required(VERSION 3.16)
project(_)

# -------------------------------------------------------------
# Import aoe cmake kit
include(FetchContent)
FetchContent_Declare(aoe_cmake_kit GIT_REPOSITORY https://github.com/Yarten/aoe_cmake_kit.git GIT_TAG main)
FetchContent_MakeAvailable(aoe_cmake_kit)

# -------------------------------------------------------------
# Define the project
aoe_project(
    NAME    readerwriterqueue
    VERSION 1.0.0
)

# Create the interface library
aoe_add_library(${PROJECT_NAME})

# Complete the project
aoe_project_complete()
