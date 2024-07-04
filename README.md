## livox_repub

## Overview

There are two types of point cloud topics sent by the livox LiDAR. One is the CustomMsg format customized by Livox, and the other is the pointcloud2 format converted from the CustomMsg format. You can refer to [configuration instructions](https://github.com/Livox-SDK/livox_ros_driver) .

This code converts the **CustomMsg format** point cloud into **pointcloud2 format** and displays it in rviz.


## Compiling

Compile using the catkin_tools package via:
```
mkdir -p livox_repub/src
cd livox_repub/src
git clone https://github.com/Shidabot/livox_repub.git
cd ..
catkin_make
```

## Execution

After compiling, source the workspace and execute via:

```
roslaunch livox_repub run.launch
rosbag play your.bag
```

## Result

![image](https://github.com/Shidabot/livox_repub/assets/67732407/97d01f13-1d6a-4fad-a1d4-cb950d8cd159)

