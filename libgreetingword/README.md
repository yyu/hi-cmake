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
