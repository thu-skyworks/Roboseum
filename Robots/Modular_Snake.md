# Modular Snake
tag: *Biorobotics Lab CMU* *仿生* *地面*

---

![SEA-Snake](../meta/pic/SEA_Snake.jpeg)

Fig. Modular Snake🐍

蛇形机器人由CMU的Howie Choset带领的Biorobotics Lab开发。其最大的亮点是模块化可拼接的身体。
## 硬件
蛇形机器人的硬件采用模块化的电机连接而成，分为头模块，尾巴模块和躯干模块。模块之间采用Ethernet通讯，供电采用串接方式。即，每个模块都有10个Pogo pin和10个焊盘，用于连接前、后的模块，其中2个pin为供电，另外8个pin为ethernet的8个通讯io。每个模块都带有自己的独立控制器，采用STM32F1系列。

- 头模块有探照灯和摄像头。
- 躯干模块有一个运动自由度，由maxon电机，编码器，惯导模块等组成，这部分构成了机器蛇运动和控制的核心。
- 尾部模块工业连接头拖出总控制线，连接到控制箱进行控制。

## 应用场景
用于军事探测，可进行管道内壁，树干外壁的攀爬

可作为多自由度机械臂，进行空间的操作

## TODO
研究其步态，包括 前进，左右移动，转向，横滚，爬树

## 拓展
[机器人链接](http://biorobotics.ri.cmu.edu/projects/modsnake/)

[视频 Modular Snake](https://www.youtube.com/watch?v=kNH0eAqz_WU&list=PLfxH9gJUcI6GG0fK4st2L8X_IJWhwlzzb&index=6)
