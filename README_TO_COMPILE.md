## Compiling
1) Download the "libstudxml" third party Git SubModule (Use GitKraken, it list the submodules on the left panel)
2) Create a "build" directory
3) Edit the File CMakeLists.txt
Compile as a static library:
option(STATIC "Set to ON to build xlnt as a static library instead of a shared library" ON)
Use C++17
set(XLNT_CXX_LANG "17" CACHE STRING "c++ language features to compile with")
4) Change to the "build" directory.
5) Configure the Makefile
cmake ..
6) Compile the library (use 4 parallel processes)
make -j 4

