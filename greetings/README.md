## on MacOS

`greetings$` **`lh`**

    total 16
    drwxr-xr-x  16 yy  staff   512B Jul 23 22:59 CMakeFiles
    -rw-r--r--   1 yy  staff   217B Jul 23 22:59 CMakeLists.txt
    -rw-r--r--   1 yy  staff   148B Jul 23 23:00 main.cpp

`greetings$` **`cmake .`**

    -- The C compiler identification is AppleClang 9.1.0.9020039
    -- The CXX compiler identification is AppleClang 9.1.0.9020039
    -- Check for working C compiler: /Library/Developer/CommandLineTools/usr/bin/cc
    -- Check for working C compiler: /Library/Developer/CommandLineTools/usr/bin/cc -- works
    -- Detecting C compiler ABI info
    -- Detecting C compiler ABI info - done
    -- Detecting C compile features
    -- Detecting C compile features - done
    -- Check for working CXX compiler: /Library/Developer/CommandLineTools/usr/bin/c++
    -- Check for working CXX compiler: /Library/Developer/CommandLineTools/usr/bin/c++ -- works
    -- Detecting CXX compiler ABI info
    -- Detecting CXX compiler ABI info - done
    -- Detecting CXX compile features
    -- Detecting CXX compile features - done
    -- Configuring done
    -- Generating done
    -- Build files have been written to: /Users/yy/___/src/github/hi-cmake/greetings

`greetings$` **`make`**

    Scanning dependencies of target greetings
    [ 50%] Building CXX object CMakeFiles/greetings.dir/main.cpp.o
    [100%] Linking CXX executable greetings
    [100%] Built target greetings

`greetings$` **`lh`**

    total 120
    -rw-r--r--   1 yy  staff    13K Jul 23 23:15 CMakeCache.txt
    drwxr-xr-x  16 yy  staff   512B Jul 23 23:15 CMakeFiles
    -rw-r--r--   1 yy  staff   217B Jul 23 22:59 CMakeLists.txt
    -rw-r--r--   1 yy  staff   4.8K Jul 23 23:15 Makefile
    -rw-r--r--   1 yy  staff   1.4K Jul 23 23:15 cmake_install.cmake
    -rwxr-xr-x   1 yy  staff    20K Jul 23 23:15 greetings
    -rw-r--r--   1 yy  staff   148B Jul 23 23:00 main.cpp

`greetings$` **`./greetings `**

    I said: hello, Jeff!

## on Ubuntu

$ (mkdir build && cd build && cmake ../greetings && make VERBOSE=1 && sudo ldconfig && ./greetings)

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
    -- Build files have been written to:
    /home/.../hi-cmake/build
    ¶
    /usr/bin/cmake
    -H/home/.../hi-cmake/greetings
    -B/home/.../hi-cmake/build
    --check-build-system CMakeFiles/Makefile.cmake 0
    /usr/bin/cmake -E cmake_progress_start
    /home/.../hi-cmake/build/CMakeFiles
    /home/.../hi-cmake/build/CMakeFiles/progress.marks
    make -f CMakeFiles/Makefile2 all
    make[1]: Entering directory
    '/home/.../hi-cmake/build'
    make -f CMakeFiles/greetings.dir/build.make
    CMakeFiles/greetings.dir/depend
    make[2]: Entering directory
    '/home/.../hi-cmake/build'
    cd /home/.../hi-cmake/build &&
    /usr/bin/cmake -E cmake_depends "Unix Makefiles"
    /home/.../hi-cmake/greetings
    /home/.../hi-cmake/greetings
    /home/.../hi-cmake/build
    /home/.../hi-cmake/build
    /home/.../hi-cmake/build/CMakeFiles/greetings.dir/DependInfo.cmake
    --color=
    Dependee
    "/home/.../hi-cmake/build/CMakeFiles/greetings.dir/DependInfo.cmake"
    is newer than depender
    "/home/.../hi-cmake/build/CMakeFiles/greetings.dir/depend.internal".
    Dependee
    "/home/.../hi-cmake/build/CMakeFiles/CMakeDirectoryInformation.cmake"
    is newer than depender
    "/home/.../hi-cmake/build/CMakeFiles/greetings.dir/depend.internal".
    Scanning dependencies of target greetings
    make[2]: Leaving directory
    '/home/.../hi-cmake/build'
    make -f CMakeFiles/greetings.dir/build.make
    CMakeFiles/greetings.dir/build
    make[2]: Entering directory
    '/home/.../hi-cmake/build'
    [ 50%] Building CXX object CMakeFiles/greetings.dir/main.cpp.o
    /usr/bin/c++  
    -I/home/.../hi-cmake/greetings/../libgreetingword 
    -std=gnu++11 -o CMakeFiles/greetings.dir/main.cpp.o -c
    /home/.../hi-cmake/greetings/main.cpp
    [100%] Linking CXX executable greetings
    /usr/bin/cmake -E cmake_link_script CMakeFiles/greetings.dir/link.txt
    --verbose=1
    /usr/bin/c++     CMakeFiles/greetings.dir/main.cpp.o  -o greetings
    -lgreetingword 
    make[2]: Leaving directory
    '/home/.../hi-cmake/build'
    [100%] Built target greetings
    make[1]: Leaving directory
    '/home/.../hi-cmake/build'
    /usr/bin/cmake -E cmake_progress_start
    /home/.../hi-cmake/build/CMakeFiles 0
    ¶
    I said: hello, Jeff!
