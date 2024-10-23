cmake_minimum_required(VERSION 3.10)
project(FilesApp)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -O3")

set(EMSCRIPTEN_FLAGS 
    -sLINKABLE=1 
    -sEXPORT_ALL=1 
    -sFORCE_FILESYSTEM=1 
)

add_executable(FilesApp Files.c)

set_target_properties(FilesApp PROPERTIES 
    OUTPUT_NAME "Files"
    SUFFIX ".wasm"
)

target_link_options(FilesApp PRIVATE ${EMSCRIPTEN_FLAGS})