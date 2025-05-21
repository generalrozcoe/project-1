
cmake_minimum_required(VERSION 3.13)

# initialize the SDK based on /home/wasabi/pico/pico-sdk
# note: this must happen before project()

project(main C CXX ASM)
set(CMAKE_C_STANDARD 11)
set(CMAKE_CXX_STANDARD 17)

# initialize the Raspberry Pi Pico SDK

add_executable(main
    src/main.cpp
    )

target_include_directories( main PRIVATE
include
)
target_link_libraries(main

)