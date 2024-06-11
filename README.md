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

**Frames**

<img src="photos/frames.png" style="width: 100%; height: 100%;">

**Map in Gazebo**

<img src="photos/map.png" style="width: 75%; height: 75%;">

**Map in RViZ**
You should delete the entire sensor visualizations, then select '2D Pose Estimate' and click on the map at the origin (0,0) like TF coordinates.

<img src="photos/map_inst_2.png" style="width: 75%; height: 75%;">

Add Pose - /optimized_pose

<img src="photos/map_est.png" style="width: 75%; height: 75%;">
