cmake_minimum_required(VERSION 3.0)

project(base64 VERSION 0.1.0)

add_library(base64 decode.c encode.c)

install(TARGETS base64
        RUNTIME DESTINATION "bin"
        LIBRARY DESTINATION "lib"
        ARCHIVE DESTINATION "lib")

install(FILES include/b64.h DESTINATION "include")
