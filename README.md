**Results:**

# SLAM: https://youtu.be/OBFY93SkfI0
# NAV2: https://youtu.be/dDSp_8K_5yw

**Packages:**

1. **car4_description**: robot model in URDF xacro
2. **car4_bringup**: Gazebo and RVIZ simulation, navigation2


**How to run:**

**build:**

`colcon build`

`source install/setup.bash`

**Generate a Map with slam_toolbox**

**Terminal 1:** Running simulation in Gazebo and RVIZ
```bash
ros2 launch car4_bringup car4_gazebo.launch.xml
```
**Terminal 2:** Controlling the robot
```bash
ros2 run teleop_twist_keyboard teleop_twist_keyboard
```
**Terminal 3:** Add map in RViZ displays. Running slam
```bash
ros2 launch slam_toolbox online_async_launch.py params_file:=mapper_params_online_async.yaml use_sim_time:=True
```
**Terminal 4:** save your map 
```bash
ros2 run nav2_map_server map_saver_cli -f name_your_map 
```

**ROS2 Nav2 Navigation**

**Terminal 1:** Running simulation in Gazebo and RVIZ 
```bash
ros2 launch car4_bringup navigation2.launch.py
```
select '2D Pose Estimate' and click on the map at the origin (0,0) like TF coordinates and next select Nav2 Goal and click where you want on the map

<img src="photos/pose2f.png" style="width: 65%; height: 65%;">

**Robot Model**

<img src="photos/model.png" style="width: 50%; height: 50%;"> <img src="photos/model.gif" style="width: 84%; height: 84%;">

**Frames & graph**

<img src="photos/frames.png" style="width: 50%; height: 50%;"><img src="photos/modelcar.svg" style="width: 50%; height: 50%;">

**Worlds in Gazebo**

**Track 1 easy**

<img src="photos/map1.png" style="width: 75%; height: 75%;">

**Track 2 medium**

<img src="photos/map2.png" style="width: 75%; height: 75%;">

**Track 3 hard**

<img src="photos/map3.png" style="width: 75%; height: 75%;">

**Generate a Map with slam_toolbox**

<img src="photos/lev2.png" style="width: 50%; height: 50%;"><img src="photos/lev2g.png" style="width: 48%; height: 48%;">

**Map after slam**

<img src="photos/maprviz.png" style="width: 70%; height: 70%;">

**ROS2 Nav2 Navigation**

<img src="photos/res2.png" style="width: 75%; height: 75%;">

**graph model with nav2**

<img src="photos/navi2.svg" style="width: 75%; height: 75%;">

