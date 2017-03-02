# maple-lite
目录结构
hardware
|-BOM
|-PCB
|-SCH

software
|-ArduCopter12M.bin
|-github

photo

BOM：PCB文件BOM
PCB：PCB源文件
SCH：原理图

ArduCopter12M.bin： 
编译ok的镜像文件，使用jlink、stlink通过jtag口直接烧写到0x08000000（flash起始地址），复位运行
github：
上传到github的源代码，可以下载后自行编译，详细参考源码README.mk

*注：晶振默认代码使用12M，如果使用其他型号请参考如下提交：
commit 90ecd17823091bf15e07f1a0bead99297502ef35
Author: solinguo <552002499@qq.com>
Date:   Sat Feb 11 23:43:20 2017 +0800

    add RCC_PLLMUL_6 support

