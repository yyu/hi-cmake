`$` **`mkdir build && cd build && cmake ../helloworld`**

    -- The C compiler identification is GNU 7.3.0
    -- The CXX compiler identification is GNU 7.3.0
    -- Check for working C compiler: /usr/bin/cc
    -- Check for working C compiler: /usr/bin/cc -- works
    -- Detecting C compiler ABI info
    -- Detecting C compiler ABI info - done
    -- Detecting C compile features
    -- Detecting C compile features - done
    -- Check for working CXX compiler: /usr/bin/c++
    -- Check for working CXX compiler: /usr/bin/c++ -- works
    -- Detecting CXX compiler ABI info
    -- Detecting CXX compiler ABI info - done
    -- Detecting CXX compile features
    -- Detecting CXX compile features - done
    -- Configuring done
    -- Generating done
    -- Build files have been written to: /home/ubuntu/__a__/cross-compile-raspi/hi-cmake/build

`$` **`make VERBOSE=1`**

    /usr/bin/cmake -H/home/ubuntu/__a__/cross-compile-raspi/hi-cmake/helloworld -B/home/ubuntu/__a__/cross-compile-raspi/hi-cmake/build --check-build-system CMakeFiles/Makefile.cmake 0
    /usr/bin/cmake -E cmake_progress_start /home/ubuntu/__a__/cross-compile-raspi/hi-cmake/build/CMakeFiles /home/ubuntu/__a__/cross-compile-raspi/hi-cmake/build/CMakeFiles/progress.marks
    make -f CMakeFiles/Makefile2 all
    make[1]: Entering directory '/home/ubuntu/__a__/cross-compile-raspi/hi-cmake/build'
    make -f CMakeFiles/helloworld.dir/build.make CMakeFiles/helloworld.dir/depend
    make[2]: Entering directory '/home/ubuntu/__a__/cross-compile-raspi/hi-cmake/build'
    cd /home/ubuntu/__a__/cross-compile-raspi/hi-cmake/build && /usr/bin/cmake -E cmake_depends "Unix Makefiles" /home/ubuntu/__a__/cross-compile-raspi/hi-cmake/helloworld /home/ubuntu/__a__/cross-compile-raspi/hi-cmake/helloworld /home/ubuntu/__a__/cross-compile-raspi/hi-cmake/build /home/ubuntu/__a__/cross-compile-raspi/hi-cmake/build /home/ubuntu/__a__/cross-compile-raspi/hi-cmake/build/CMakeFiles/helloworld.dir/DependInfo.cmake --color=
    Dependee "/home/ubuntu/__a__/cross-compile-raspi/hi-cmake/build/CMakeFiles/helloworld.dir/DependInfo.cmake" is newer than depender "/home/ubuntu/__a__/cross-compile-raspi/hi-cmake/build/CMakeFiles/helloworld.dir/depend.internal".
    Dependee "/home/ubuntu/__a__/cross-compile-raspi/hi-cmake/build/CMakeFiles/CMakeDirectoryInformation.cmake" is newer than depender "/home/ubuntu/__a__/cross-compile-raspi/hi-cmake/build/CMakeFiles/helloworld.dir/depend.internal".
    Scanning dependencies of target helloworld
    make[2]: Leaving directory '/home/ubuntu/__a__/cross-compile-raspi/hi-cmake/build'
    make -f CMakeFiles/helloworld.dir/build.make CMakeFiles/helloworld.dir/build
    make[2]: Entering directory '/home/ubuntu/__a__/cross-compile-raspi/hi-cmake/build'
    [ 50%] Building CXX object CMakeFiles/helloworld.dir/main.cpp.o
    /usr/bin/c++    -std=gnu++11 -o CMakeFiles/helloworld.dir/main.cpp.o -c /home/ubuntu/__a__/cross-compile-raspi/hi-cmake/helloworld/main.cpp
    [100%] Linking CXX executable helloworld
    /usr/bin/cmake -E cmake_link_script CMakeFiles/helloworld.dir/link.txt --verbose=1
    /usr/bin/c++     CMakeFiles/helloworld.dir/main.cpp.o  -o helloworld 
    make[2]: Leaving directory '/home/ubuntu/__a__/cross-compile-raspi/hi-cmake/build'
    [100%] Built target helloworld
    make[1]: Leaving directory '/home/ubuntu/__a__/cross-compile-raspi/hi-cmake/build'
    /usr/bin/cmake -E cmake_progress_start /home/ubuntu/__a__/cross-compile-raspi/hi-cmake/build/CMakeFiles 0

`$` **`tree`**

    .
    ├── CMakeCache.txt
    ├── CMakeFiles
    │   ├── 3.10.2
    │   │   ├── CMakeCCompiler.cmake
    │   │   ├── CMakeCXXCompiler.cmake
    │   │   ├── CMakeDetermineCompilerABI_C.bin
    │   │   ├── CMakeDetermineCompilerABI_CXX.bin
    │   │   ├── CMakeSystem.cmake
    │   │   ├── CompilerIdC
    │   │   │   ├── a.out
    │   │   │   ├── CMakeCCompilerId.c
    │   │   │   └── tmp
    │   │   └── CompilerIdCXX
    │   │       ├── a.out
    │   │       ├── CMakeCXXCompilerId.cpp
    │   │       └── tmp
    │   ├── cmake.check_cache
    │   ├── CMakeDirectoryInformation.cmake
    │   ├── CMakeOutput.log
    │   ├── CMakeTmp
    │   ├── feature_tests.bin
    │   ├── feature_tests.c
    │   ├── feature_tests.cxx
    │   ├── helloworld.dir
    │   │   ├── build.make
    │   │   ├── cmake_clean.cmake
    │   │   ├── CXX.includecache
    │   │   ├── DependInfo.cmake
    │   │   ├── depend.internal
    │   │   ├── depend.make
    │   │   ├── flags.make
    │   │   ├── link.txt
    │   │   ├── main.cpp.o
    │   │   └── progress.make
    │   ├── Makefile2
    │   ├── Makefile.cmake
    │   ├── progress.marks
    │   └── TargetDirectories.txt
    ├── cmake_install.cmake
    ├── helloworld
    └── Makefile

    8 directories, 33 files

`$` **`./helloworld `**

    Hello freakin' world
