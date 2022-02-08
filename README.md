# p450_experiment

本仓库内容为Prometheus p450飞机实机存储库

注：根据实机需要，本仓库内容需要搭配Prometheus开源代码以及rplidar/realsense t265/d435i等传感器驱动使用。

## Prometheus p450无人机板载计算机配置内容

### 需要配置的ros工作空间内容

|源代码工程名称|作用|配置方式|源代码GitHub下载链接|
|-|-|-|-|
|Prometheus|无人机仿真及核心算法库|参考Prometheus教程编译安装|https://github.com/amov-lab/Prometheus|
|p450_experiment|无人机实机启动所需要的配置文件|新建一个ros工作空间，放入src文件夹内并编译安装||
|realsense-ros|realsense相机的ros驱动文件|新建一个ros工作空间，放入src文件夹内并编译安装|https://github.com/IntelRealSense/realsense-ros|
|vision-to-mavros|realsense相机的位姿信息转化为mavros位姿信息|同上，建议将realsense-ros与本项放在同一个ros工作空间的src文件夹内并编译安装|https://github.com/thien94/vision_to_mavros|
|rplidar-ros|激光雷达的ros驱动文件|新建一个ros工作空间，放入src文件夹内并编译安装|https://github.com/Slamtec/rplidar_ros|

### 需要配置的硬件驱动

|驱动名称|作用|配置方式|源代码GitHub下载链接|
|-|-|-|-|
|realsense驱动|realsense相机驱动|Linux编译安装|https://github.com/IntelRealSense/librealsense|
