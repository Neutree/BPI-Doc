# 用microbit按钮控制电机

## 程序功能

1. 启动或复位时停车。
2. 同时按下AB按钮直行。
3. 按下A按钮右转。
4. 按下B按钮左转。

## 例程

<div style="position:relative;height:0;padding-bottom:100%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_8MqMbVYFbXev" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>

> 点击例程中的 Edit 编辑 即可作为一个项目在makecode编辑器中打开，点击下方 Downlord 下载 即可通过USB下载进micro:bit中。

## 设计说明

在[硬件浅析与调试：驱动电路](../hardware/analysis&calibrate.html#驱动电路)中后半部分有提到，驱动电路中有设计一个切换开关，可以将驱动电路由LM393电压比较器控制切换到由micro:bit控制。而micro:bit控制驱动电路的方法，和LM393电压比较器相同，低电平启动，高电平停止。