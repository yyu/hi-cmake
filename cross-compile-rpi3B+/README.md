`$` **`tree -L 3 /opt/pi`**

    /opt/pi
    ├── rootfs
    │   ├── lib
    │   │   ├── arm-linux-gnueabihf
    │   │   ├── console-setup
    │   │   ├── cpp -> /etc/alternatives/cpp
    │   │   ├── crda
    │   │   ├── dhcpcd
    │   │   ├── firmware
    │   │   ├── ifupdown
    │   │   ├── init
    │   │   ├── klibc-z-GH4vbo1mvhrmAe8pZWxAgGeP0.so
    │   │   ├── ld-linux-armhf.so.3 -> arm-linux-gnueabihf/ld-2.24.so
    │   │   ├── ld-linux.so.3 -> /lib/ld-linux-armhf.so.3
    │   │   ├── libnih-dbus.so.1 -> libnih-dbus.so.1.0.0
    │   │   ├── libnih-dbus.so.1.0.0
    │   │   ├── libnih.so.1 -> libnih.so.1.0.0
    │   │   ├── libnih.so.1.0.0
    │   │   ├── lsb
    │   │   ├── modprobe.d
    │   │   ├── modules
    │   │   ├── resolvconf
    │   │   ├── systemd
    │   │   ├── terminfo
    │   │   └── udev
    │   └── usr
    │       ├── bin
    │       ├── games
    │       ├── include
    │       ├── lib
    │       ├── local
    │       ├── man
    │       ├── sbin
    │       ├── share
    │       └── src
    └── tools
        ├── arm-bcm2708
        │   ├── arm-bcm2708hardfp-linux-gnueabi
        │   ├── arm-bcm2708-linux-gnueabi
        │   ├── arm-linux-gnueabihf -> arm-rpi-4.9.3-linux-gnueabihf
        │   ├── arm-rpi-4.9.3-linux-gnueabihf
        │   ├── gcc-linaro-arm-linux-gnueabihf-raspbian
        │   └── gcc-linaro-arm-linux-gnueabihf-raspbian-x64
        ├── armstubs
        │   ├── armstub7.S
        │   ├── armstub8.S
        │   ├── armstub.S
        │   ├── bin2c.c
        │   └── Makefile
        ├── configs
        │   ├── arm-rpi-4.9.3-linux-gnueabihf.config
        │   ├── bcm2708-ct-ng.config
        │   ├── bcm2708hardfp-ct-ng.config
        │   ├── ct-nt-version
        │   └── gcc-linaro-arm-linux-gnueabihf-raspbian
        ├── mkimage
        │   ├── args-uncompressed.txt
        │   ├── boot-uncompressed.txt
        │   ├── first32k.bin
        │   ├── imagetool-uncompressed.py
        │   └── README
        ├── pkg
        │   ├── rpi_ref-root-nodata.tgz
        │   └── scripts-bin.tgz
        ├── sysidk
        ├── test_code
        │   ├── main.c
        │   ├── Makefile
        │   └── Readme.md
        └── usbboot
            └── Readme.md

    40 directories, 30 files

`$` **`mkdir build && cd build && cmake -DCMAKE_TOOLCHAIN_FILE=../cross-compile-rpi3B+/pi.cmake ../helloworld/`**

-- The C compiler identification is GNU 4.9.3
-- The CXX compiler identification is GNU 4.9.3
-- Check for working C compiler: /opt/pi/tools/arm-bcm2708/arm-rpi-4.9.3-linux-gnueabihf/bin/arm-linux-gnueabihf-gcc
-- Check for working C compiler: /opt/pi/tools/arm-bcm2708/arm-rpi-4.9.3-linux-gnueabihf/bin/arm-linux-gnueabihf-gcc -- works
-- Detecting C compiler ABI info
-- Detecting C compiler ABI info - done
-- Detecting C compile features
-- Detecting C compile features - done
-- Check for working CXX compiler: /opt/pi/tools/arm-bcm2708/arm-rpi-4.9.3-linux-gnueabihf/bin/arm-linux-gnueabihf-g++
-- Check for working CXX compiler: /opt/pi/tools/arm-bcm2708/arm-rpi-4.9.3-linux-gnueabihf/bin/arm-linux-gnueabihf-g++ -- works
-- Detecting CXX compiler ABI info
-- Detecting CXX compiler ABI info - done
-- Detecting CXX compile features
-- Detecting CXX compile features - done
-- Configuring done
-- Generating done
-- Build files have been written to: /.../hi-cmake/build

`$` **`make`**

    Scanning dependencies of target helloworld
    [ 50%] Building CXX object CMakeFiles/helloworld.dir/main.cpp.o
    [100%] Linking CXX executable helloworld
    [100%] Built target helloworld

