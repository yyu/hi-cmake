## on MacOS

`libgreetingword$` **`lh`**

    total 24
    -rw-r--r--  1 yy  staff   207B Jul 23 22:55 CMakeLists.txt
    -rw-r--r--  1 yy  staff   117B Jul 23 22:55 greetingword.cpp
    -rw-r--r--  1 yy  staff   134B Jul 23 22:55 greetingword.h

`libgreetingword$` **`cmake .`**

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
    -- Build files have been written to: /path/to/libgreetingword

`libgreetingword$` **`lh`**

    total 80
    -rw-r--r--   1 yy  staff    13K Jul 23 22:57 CMakeCache.txt
    drwxr-xr-x  15 yy  staff   480B Jul 23 22:57 CMakeFiles
    -rw-r--r--   1 yy  staff   207B Jul 23 22:55 CMakeLists.txt
    -rw-r--r--   1 yy  staff   7.2K Jul 23 22:57 Makefile
    -rw-r--r--   1 yy  staff   2.4K Jul 23 22:57 cmake_install.cmake
    -rw-r--r--   1 yy  staff   117B Jul 23 22:55 greetingword.cpp
    -rw-r--r--   1 yy  staff   134B Jul 23 22:55 greetingword.h

`libgreetingword$` **`make`**

    Scanning dependencies of target greetingword
    [ 50%] Building CXX object CMakeFiles/greetingword.dir/greetingword.cpp.o
    [100%] Linking CXX shared library libgreetingword.dylib
    [100%] Built target greetingword

`libgreetingword$` **`make install`**

    [100%] Built target greetingword
    Install the project...
    -- Install configuration: ""
    -- Installing: /usr/local/lib/libgreetingword.dylib

## on Ubuntu

$ (mkdir build-lib && cd build-lib && cmake ../libgreetingword && make VERBOSE=1 && sudo make install VERBOSE=1)

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
    /home/.../hi-cmake/build-lib
    ¶
    /usr/bin/cmake
    -H/home/.../hi-cmake/libgreetingword
    -B/home/.../hi-cmake/build-lib
    --check-build-system CMakeFiles/Makefile.cmake 0
    /usr/bin/cmake -E cmake_progress_start
    /home/.../hi-cmake/build-lib/CMakeFiles
    /home/.../hi-cmake/build-lib/CMakeFiles/progress.marks
    make -f CMakeFiles/Makefile2 all
    make[1]: Entering directory
    '/home/.../hi-cmake/build-lib'
    make -f CMakeFiles/greetingword.dir/build.make
    CMakeFiles/greetingword.dir/depend
    make[2]: Entering directory
    '/home/.../hi-cmake/build-lib'
    cd /home/.../hi-cmake/build-lib &&
    /usr/bin/cmake -E cmake_depends "Unix Makefiles"
    /home/.../hi-cmake/libgreetingword
    /home/.../hi-cmake/libgreetingword
    /home/.../hi-cmake/build-lib
    /home/.../hi-cmake/build-lib
    /home/.../hi-cmake/build-lib/CMakeFiles/greetingword.dir/DependInfo.cmake
    --color=
    Dependee
    "/home/.../hi-cmake/build-lib/CMakeFiles/greetingword.dir/DependInfo.cmake"
    is newer than depender
    "/home/.../hi-cmake/build-lib/CMakeFiles/greetingword.dir/depend.internal".
    Dependee
    "/home/.../hi-cmake/build-lib/CMakeFiles/CMakeDirectoryInformation.cmake"
    is newer than depender
    "/home/.../hi-cmake/build-lib/CMakeFiles/greetingword.dir/depend.internal".
    Scanning dependencies of target greetingword
    make[2]: Leaving directory
    '/home/.../hi-cmake/build-lib'
    make -f CMakeFiles/greetingword.dir/build.make
    CMakeFiles/greetingword.dir/build
    make[2]: Entering directory
    '/home/.../hi-cmake/build-lib'
    [ 50%] Building CXX object
    CMakeFiles/greetingword.dir/greetingword.cpp.o
    /usr/bin/c++  -Dgreetingword_EXPORTS  -fPIC   -std=gnu++11 -o
    CMakeFiles/greetingword.dir/greetingword.cpp.o -c
    /home/.../hi-cmake/libgreetingword/greetingword.cpp
    [100%] Linking CXX shared library libgreetingword.so
    /usr/bin/cmake -E cmake_link_script CMakeFiles/greetingword.dir/link.txt
    --verbose=1
    /usr/bin/c++ -fPIC   -shared -Wl,-soname,libgreetingword.so -o
    libgreetingword.so CMakeFiles/greetingword.dir/greetingword.cpp.o
    make[2]: Leaving directory
    '/home/.../hi-cmake/build-lib'
    [100%] Built target greetingword
    make[1]: Leaving directory
    '/home/.../hi-cmake/build-lib'
    /usr/bin/cmake -E cmake_progress_start
    /home/.../hi-cmake/build-lib/CMakeFiles 0
    ¶
    /usr/bin/cmake
    -H/home/.../hi-cmake/libgreetingword
    -B/home/.../hi-cmake/build-lib
    --check-build-system CMakeFiles/Makefile.cmake 0
    /usr/bin/cmake -E cmake_progress_start
    /home/.../hi-cmake/build-lib/CMakeFiles
    /home/.../hi-cmake/build-lib/CMakeFiles/progress.marks
    make -f CMakeFiles/Makefile2 all
    make[1]: Entering directory
    '/home/.../hi-cmake/build-lib'
    make -f CMakeFiles/greetingword.dir/build.make
    CMakeFiles/greetingword.dir/depend
    make[2]: Entering directory
    '/home/.../hi-cmake/build-lib'
    cd /home/.../hi-cmake/build-lib &&
    /usr/bin/cmake -E cmake_depends "Unix Makefiles"
    /home/.../hi-cmake/libgreetingword
    /home/.../hi-cmake/libgreetingword
    /home/.../hi-cmake/build-lib
    /home/.../hi-cmake/build-lib
    /home/.../hi-cmake/build-lib/CMakeFiles/greetingword.dir/DependInfo.cmake
    --color=
    make[2]: Leaving directory
    '/home/.../hi-cmake/build-lib'
    make -f CMakeFiles/greetingword.dir/build.make
    CMakeFiles/greetingword.dir/build
    make[2]: Entering directory
    '/home/.../hi-cmake/build-lib'
    make[2]: Nothing to be done for 'CMakeFiles/greetingword.dir/build'.
    make[2]: Leaving directory
    '/home/.../hi-cmake/build-lib'
    [100%] Built target greetingword
    make[1]: Leaving directory
    '/home/.../hi-cmake/build-lib'
    /usr/bin/cmake -E cmake_progress_start
    /home/.../hi-cmake/build-lib/CMakeFiles 0
    make -f CMakeFiles/Makefile2 preinstall
    make[1]: Entering directory
    '/home/.../hi-cmake/build-lib'
    make[1]: Nothing to be done for 'preinstall'.
    make[1]: Leaving directory
    '/home/.../hi-cmake/build-lib'
    Install the project...
    /usr/bin/cmake -P cmake_install.cmake
    -- Install configuration: ""
    -- Installing: /usr/local/lib/libgreetingword.so

$ sudo ldconfig
