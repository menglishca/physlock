cmake_minimum_required(VERSION 3.13)
project(physlock)

set(CMAKE_C_STANDARD 99)

add_executable(physlock main.c options.c config.def.h issue.c session.c util.c vt.c physlock.h)
set(CMAKE_C_FLAGS "-lpam_misc -lpam")