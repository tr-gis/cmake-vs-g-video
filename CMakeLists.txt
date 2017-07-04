cmake_minimum_required(VERSION 2.8.9)
project(ctest)
 
#Bring the headers, such as Student.h into the project
include_directories(include)
 
#Can manually add the sources using the set command as follows:
#set(SOURCES src/mainapp.cpp src/Student.cpp)
 
#However, the file(GLOB...) allows for wildcard additions:
#This will add all the files ending with .cpp inside src as source files
file(GLOB SOURCES "src/*.cpp")
 
#syntax:add_executable(executable_name list_of_source_files)
add_executable(exec ${SOURCES})
