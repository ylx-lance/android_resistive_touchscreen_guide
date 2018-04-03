# resistive_touchscreen_guide
Android电阻屏驱动移植指导方案

一个Linux的触摸屏驱动其实包含三个部分：
1. LCD设备驱动，负责图像显示的部分；
2. 触摸驱动，负责触摸屏下触摸板的响应；
3. 背光驱动，负责显示屏亮度的调节。


本文的余下部分将会分别从这三个部分介绍电阻触摸屏在Android系统上的移植细节。
- 电阻触摸屏型号：AM-800600P4TMQW-TB0H
- 电阻芯片：tsc2007
- 分辨率：800x600
- Android源码版本：Android 5.1
- Android开发板型号：NanoPI T2(友善之臂提供)
