cmake_minimum_required(VERSION 2.8)

set(PROJ_HASHTABLE hashtable)

project(${PROJ_HASHTABLE} C)
set(SOURCE_FILES main.c test.h hashfunc.h  hashtable.h hashtable.c murmur.c murmur.h timer.h)
set(CMAKE_C_FLAGS "-std=c99 -Wall")

include_directories(/usr/include /usr/include/x86_64-linux-gnu)

add_executable(hashtable ${SOURCE_FILES})


