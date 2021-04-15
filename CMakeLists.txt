cmake_minimum_required(VERSION 3.16)
project(untitled1 C)

set(CMAKE_C_STANDARD 99)

aux_source_directory(bzip2 SOURCE)

include_directories(bzip2)

add_executable(bspatch  bspatch.c ${SOURCE})  # 生成可执行文件