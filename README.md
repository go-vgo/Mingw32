# Mingw32
Download Mingw32, set environment variables

The current version does not require this step. /* Download win32, copy win32 inside the file (don't copy win32 folder) to Mingw/lib/gcc/mingw32/4.8.1/include, because the download the path is different (
    mingw/lib/gcc/i686-w64-mingw32/4.8.1/include or other
)*/

Download zlib and libpng-1.5.27, generate libpng.a, copy to Mingw/lib

### Generate libpng.a:

    Copy scripts/pnglibconf.h.prebuilt to pnglibconf.h

    And run in cmd:
        copy scripts\makefile.gcc makefile.gcc
        mingw32-make -f makefile.gcc

### If can't work, you can try:

    Copy win32 inside the file to Mingw/mingw32/lib/gcc/mingw32/4.8.1/include

    Copy libpng.a to Mingw/mingw32/lib



# 中文文档

下载 32 位的 Mingw, 并设置环境变量

当前版本不需要此步骤. /* 再把 [Mingw32](https://github.com/go-vgo/Mingw32) 里面的 win32 里面的文件 (不需要 win32 文件夹)
复制到 Mingw/lib/gcc/mingw32/4.8.1/include 里面, 路径可能因不同下载不同
(mingw/lib/gcc/i686-w64-mingw32/4.8.1/include 或者其他) */ 

下载 zlib and libpng-1.5.27, 生成 libpng.a, 复制到 Mingw/lib 

### 生成 libpng.a:

    复制 scripts/pnglibconf.h.prebuilt 到 pnglibconf.h

    在 cmd 终端运行:
        copy scripts\makefile.gcc makefile.gcc
        mingw32-make -f makefile.gcc   

