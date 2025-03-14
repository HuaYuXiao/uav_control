# px4ctrl

![HitCount](https://img.shields.io/endpoint?url=https%3A%2F%2Fhits.dwyl.com%2FHuaYuXiao%2Fpx4ctrl.json%3Fcolor%3Dpink)
![Static Badge](https://img.shields.io/badge/ROS-noetic-22314E?logo=ros)
![Static Badge](https://img.shields.io/badge/C%2B%2B-17-00599C?logo=cplusplus)
![Static Badge](https://img.shields.io/badge/Python-3.8.10-3776AB?logo=python)
![Static Badge](https://img.shields.io/badge/Ubuntu-20.04.6-E95420?logo=ubuntu)

A **ROS** package to control multi-copters with **PX4-Autopilot** & **MAVROS** platform.

## Features

1. Process **EKF2 fusion** from SLAM, Gazebo, MoCap, etc. Publish to `/mavros/vision_pose/pose`
2. Control drone to `Arm`, `Takeoff`, `Offboard`, `Move`, `Hold`, `Land`, Return, etc. Publish to `/mavros/setpoint_raw/local`
3. Process control command from path-planner, with format `quadrotor_msgs::PositionCommand`
4. Interact with a terminal to control drone, with format `easondrone_msgs::ControlCommand`

![screenshot](doc/Snipaste_2024-08-25_21-44-35.png)

Visit this [yuque doc](https://www.yuque.com/g/easonhua/nx9k7f/xuv0pnk5yxk9qw3v/collaborator/join?token=V4SM11MTCXNawO7w&source=doc_collaborator#) for detailed information.

## Launch

```sh
roslaunch px4ctrl px4ctrl.launch
```

![rosgraph.png](doc/rosgraph.png)

## Acknowledgement

Thanks for following packages:

- [Prometheus/prometheus_control](https://github.com/amov-lab/Prometheus/Modules/control)
- [XTDrone/control](https://gitee.com/robin_shaun/XTDrone/control)
- [Fast-Drone-250/px4ctrl](https://github.com/ZJU-FAST-Lab/Fast-Drone-250/src/realflight_modules/px4ctrl)

Related docs:

- [mavros wiki](https://wiki.ros.org/mavros)
- [px4 user guide](https://docs.px4.io/master/en/)
