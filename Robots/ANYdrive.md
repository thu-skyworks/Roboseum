# ANYdrive
tag: *ETHZ* *执行* *电机*
author：gzy
date：2017.11.22

---
- 图1
![](../meta/pic/ANYdrive.jpg)

ANYdrive是苏黎世理工的Robot System Lab开发的一款无刷电机，实验室利用电机开发了一款机械臂ANYpulator和机械狗ANYmal.

然后实验室拿着电机创业开办了ANYbotics，很多人都是原实验室的人，包括实验室老板。

ANYdrive最大的亮点是引入了SEA,作为一款有柔性的电机，这个性能还是非常出色的。20Nm的驱动力矩，在SEA的保护下峰值可达到40Nm。

## 硬件

#### 基本参数
- 尺寸95 x 90 mm
- 1Kg的质量
- 无刷+齿轮减速+SEA

#### 性能
- 位置精度，0.025°（这个相当高了
- 力矩控制带宽：60Hz（可以理解，SEA通常带宽都很低。作为对比，BLDC直驱的力控带宽至少上百Hz，可见SEA对电机控制频率的影响。所以这也就是为什么视频里面safe interaction的时候转速这么低，因为控制频率上不去）
- 48V供电,最大功率720W，额定功率240W
- 最大力矩40Nm，额定力矩20Nm（感觉一般，转速这么低）
- 最大峰值转速114rpm（带了减速电机，RPM太低了，这也就是为什么这个电机做的狗动作这么慢，ANYdrive视频里面转速也确实不高）
- IP67的防尘防水精度，堪比iPhone7
- 支持ROS和Ethercat通信（然而控制带宽这么低，要Ethercat有何用…）
- low-impedance torque control低阻抗控制（不明白有什么用，求讨论）

#### 控制方式
- 官方SDK还没有发布
- 我认为应该会做成ROS包与控制器通讯的形式
- 控制器支持CAN总线控制，CAN的通讯频率可以达到1Mbit/s，然而，电机执行频率跟不上的，控制频率的瓶颈是电机的响应速度
- Ethercat，不过意义不大

#### 传感器
- 绝对位置编码器

## 应用场景
- 高精度的位置和力控制
- 可以抵抗外力，有一定鲁棒性（SEA的功劳）
- 力存储（SEA的功劳）
- safe interaction，人机安全控制（SEA的功劳）

## 拓展
[实验室连接](http://www.rsl.ethz.ch/robots-media/actuators/anydrive.html)

[公司产品链接](https://www.anybotics.com/anydrive/)

[产品介绍PDF](../meta/datasheet/ANYdrive.pdf)