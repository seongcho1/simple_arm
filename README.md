# simple_arm_01
A mini-project for RoboND's ROS Basics Module, Lesson 02.

## ./scripts/hello

```
$ chmod u+x hello
$ cd ~/catkin_ws
$ catkin_make
$ source devel/setup.bash
$ rosrun simple_arm hello
```

## ./scripts/simple_mover

```
$ cd ~/catkin_ws
$ roslaunch simple_arm robot_spawn.launch
```

```
$ cd ~/catkin_ws
$ source devel/setup.bash
$ rosrun simple_arm simple_mover
```

## ./scripts/arm_mover

```
$ cd ~/catkin_ws
$ catkin_make
$ source devel/setup.bash
$ roslaunch simple_arm robot_spawn.launch
```

```
$ rosnode list
$ rosservice list
```

```
$ rqt_image_view /rgb_camera/image_raw
```

```
$ rosservice call /arm_mover/safe_move "joint_1: 1.57
joint_2: 1.57"
```

## ./scripts/look_away

```
$ cd ~/catkin_ws
$ catkin_make
$ source devel/setup.bash
$ roslaunch simple_arm robot_spawn.launch
```

```
$ rqt_image_view /rgb_camera/image_raw
```

```
rosservice call /arm_mover/safe_move "joint_1: 0
joint_2: 0"
```
