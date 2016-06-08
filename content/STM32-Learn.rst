STM32 Keil笔记
##############

:date: 2015-01-15 15:08
:modified: 2015-01-15 15:08
:tags: STM32,Keil
:category: STM32
:slug: stm32-keil 
:authors: htstudios
:summary: STM32

头文件
==================

Keil头文件组织方法让我一头雾水。ST提供CMSIS（Cortex-M Software Interface Standard）和标准外设驱动（STM32F10x_StdPeriph_Driver）。默认库文件是不能修改的，当你要使用这些功能或选择使用一款单片机型号时，你必须定义一些符号，例如定义 `TM32F10X_MD` 为使用的中密度STM32F10X设备、定义 `USE_STDPERIPH_DRIVER` 为使用标准外设驱动。

在使用标准外设驱动时，你必须编写 **stm32f10x_conf.h** 头文件来决定使用哪
些标准驱动，否则可能会调用Keil自带头文件导致编译失败。这个文件在ST官方
示例中存在，可以直接拷贝过来使用（别忘记修改工程头文件目录）。

编译器
==================

调试方法
==================

STM32支持多种启动方式，如果是擦写Flash，你必须重启测试程序，也可以使用Debug
直接使用Jlink（其他调试器也可能支持）在线调试。
