
cmake_minimum_required(VERSION 3.7)
set( CMAKE_VERBOSE_MAKEFILE on )
project(sqlite)
add_library(sqlite STATIC sqlite-amalgamation-3160200/sqlite3.c)
file(COPY sqlite-amalgamation-3160200/sqlite3.h DESTINATION ${CMAKEIFY_REDIST_INCLUDE_DIRECTORY})

