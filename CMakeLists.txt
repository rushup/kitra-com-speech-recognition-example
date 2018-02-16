cmake_minimum_required(VERSION 2.8 FATAL_ERROR)
project(kitra_com_audio_proj)

add_subdirectory(kitra-com-lib)
include_directories(kitra-com-lib)

set(kitra_com_example_source_files
    main.cpp
    serial.cpp
    serial.h
    )
add_executable(kitra_com_exe ${kitra_com_example_source_files})

target_link_libraries(kitra_com_exe kitra_com_lib)
