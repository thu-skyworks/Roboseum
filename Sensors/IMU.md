## IMU（Inertia Measurement Unit）

一般IMU都是6轴起步，即xyz方向的加速度计accelerometers和Pitch Roll Yaw方向角速度的陀螺仪gyroscope。
9轴IMU还加上了电子罗盘（地磁传感器，地磁计），用以获得绝对姿态。
有的IMU还有温度信息，作为某种偏差补偿。

## 互补滤波

比较著名的有Madgwick的算法，arduino官方github上有c的实现。

## Kalman滤波

最为著名的一个算法。