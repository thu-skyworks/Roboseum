# Fetch机器人平台

tag: *Fetch Robotics* *机械臂* *轮式* *地面*

author: gzy @ Dec.2018

---

- Freight移动机器人
![Freight](../meta/pic/Freight_base.png)

- Fetch & Freight
![Fetch](../meta/pic/Fetch.png)

Fetch Robotics成立于2014，2017年12月的B轮融资$25M。其核心服务：快速部署自动仓储，ioT云技术。为此团队设计了各种各样能够连上云端，进行远程控制的移动平台，和打造了一个云服务平台。

而我们关心的是其机器人产品：Freight移动机器人和Fetch机械臂。这家公司的独特之处在于拥抱开源和学术界。他们将其中两款产品写了驱动，做了文档，把平台开放出来让大家开发，这就吸引很多公司和实验室用他们的平台来进行机器人算法开发。

看起来这家公司相当有做硬件的实力，机械底盘谁都能造，但是自己造机械臂还是要勇气的。这家的产品和pr2很类似，而willow garage已经跪了。现在卖机器人是赚不了什么钱的，只能想办法和行业靠拢，做仓储物流平台像是正确的思路，公司能融到25M说明还是有市场可以赚钱。下次可以介绍一下Fetch的竞争对手，从Willow Garage脱离出来的unbounded Robotics，做的产品简直一模一样。

## 硬件

详细的硬件的参数可以在下面的拓展中有详细链接。这里主要列举几个基本量。

- 身高 1.1m
- 机械臂 7 DoF + 末端 1 DoF
- 头部 2 Dof
- 头部 RGBD相机
- 底盘 3D线激光雷达
- 底盘 6轴IMU
- 电池续航 8h

## 应用场景

家居服务，主要用于科研

## 拓展
[机器人平台文档](http://docs.fetchrobotics.com/introduction.html)，这个做的相当详细，毕竟拿出来卖的产品，还是下了功夫了。ROS的Navigation那一套和MoveIt那一套都可以拿来用，做research上手相当方便。

[机器人平台的主要参数](https://fetchrobotics.com/wp-content/uploads/2018/04/Fetch_robot_spec_overview.pdf)

[机器人平台文章2012](https://fetchrobotics.com/wp-content/uploads/2018/04/Fetch-and-Freight-Workshop-Paper.pdf)
