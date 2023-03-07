[![Security Status](https://s.murphysec.com/badge/Lmh-sys/line_ws.svg)](https://www.murphysec.com/p/Lmh-sys/line_ws)
# line_ws
## 编译
```
git clone https://github.com/Lmh-sys/line_ws
cd line_ws
catkin_make
source devel/setup.bash 
```
## 运行
**开启底盘通信**
```
cd ~/catkin_ws
./src/scout_base/scout_bringup/scripts/bringup_can2usb.bash
roslaunch scout_bringup scout_minimal.launch
```
**启动巡线**
```
roslaunch simple_follower line_follower.launch
```
