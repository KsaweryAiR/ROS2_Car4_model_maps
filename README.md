# SLAM: https://youtu.be/OBFY93SkfI0
# NAV2: https://youtu.be/dDSp_8K_5yw

**Packages:**

1. **car4_description**: robot model in URDF xacro
2. **car4_bringup**: Gazebo and RVIZ simulation, navigation2


**How to run:**

**build:**

`colcon build`

`source install/setup.bash`

**Terminal 1:** `ros2 launch car4_bringup navigation2.launch.py` 

Running simulation in Gazebo and RVIZ.

**Terminal 2:** `ros2 run teleop_twist_keyboard teleop_twist_keyboard` 

Controlling the robot.

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

