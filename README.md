# cmake-vs-g++-video

To recreate the video create three directories. src, include and build.
Place the .cpp files inside src and the .h file inside include.
Leave the build directory empty for now.
Place the CMakeLists.txt file outside these directories.

               Some_folder_name
                    |_build
                    |_include-|_student.h
                    |
                    |_src-|_main.cpp
                    |     |_student.cpp
                    |
                    |_CMakeLists.txt
Watch the video "out.ogv" for further instructions.

we use "cmake .." from inside build beacause the CMakeLists.txt file is located on level above. If the CMakeLists.txt file is in the same level we use "cmake ." 

Some notes:
take a look at the linux folder in google drive for cmake tutorial.

*)using cmake helps to keep things clean.ie; header files and src code seperately.
*)the name of the executable is the first argument in add_executable() function inside CMakeLists.txt
syntax : add_executable(executable_name list_of_source_files)
