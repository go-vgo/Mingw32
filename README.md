# Mingw32
Download Mingw32,set environment variables

Download win32 ,copy win32 inside the file(don't copy win32 Folder) to Mingw/lib/gcc/mingw32/4.8.1/include
(or mingw/lib/gcc/i686-w64-mingw32/4.8.1/include or other),Because the download the path is different

Download zlib and libpng-1.5.27,generate libpng.a,copy to Mingw/lib

###Generate libpng.a:

    Copy scripts/pnglibconf.h.prebuilt to pnglibconf.h

    And run in cmd:
        copy scripts\makefile.gcc makefile.gcc
        mingw32-make -f makefile.gcc

###If can't work, you can try:

    Copy win32 inside the file to Mingw/mingw32/lib/gcc/mingw32/4.8.1/include

    Copy libpng.a to Mingw/mingw32/lib



#中文文档

下载一个32位的Mingw,并设置环境变量

再把https://github.com/go-vgo/Mingw32 里面的win32里面的文件(不要win32文件夹)
复制到Mingw/lib/gcc/mingw32/4.8.1/include里面, 路径可能因不同下载不同
(mingw/lib/gcc/i686-w64-mingw32/4.8.1/include 或者其他)

下载zlib and libpng-1.5.27,生成 libpng.a,复制到Mingw/lib 

###生成 libpng.a:

    复制 scripts/pnglibconf.h.prebuilt 到 pnglibconf.h

    在cmd终端运行:
        copy scripts\makefile.gcc makefile.gcc
        mingw32-make -f makefile.gcc   

