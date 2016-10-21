# Mingw32
Download Mingw32

Download win32 ,copy win32 inside the file to Mingw/lib/gcc/mingw32/4.8.1/include

Download zlib and libpng-1.5.27,generate libpng.a,copy to Mingw/lib

###generate libpng.a:

    Copy scripts/pnglibconf.h.prebuilt to pnglibconf.h

    And run in cmd:
        copy scripts\makefile.gcc makefile.gcc
        mingw32-make -f makefile.gcc

###If can't work, you can try:

    Copy win32 inside the file to Mingw/mingw32/lib/gcc/mingw32/4.8.1/include

    Copy libpng.a to Mingw/mingw32/lib

