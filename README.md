Windows下生成带图标的可执行文件
==================================

这个例子只针对安装了MinGW环境的Windows系统

编译顺序：

    gcc -c 1.c -o 1.o

    windres 1.rc -O coff -o 1.res

    gcc 1.o 1.res -o 1.exe

