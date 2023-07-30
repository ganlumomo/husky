husky_gazebo
=====

### Installation
Add the heightmap model to gazebo (where gazebo is installed)
```bash
sudo cp -r models/heightmap/ /usr/share/gazebo-11/models/
```
Export realsense urdf by adding the following to bashrc:
```
export HUSKY_URDF_EXTRAS=[CATKIN WORKSPACE PATH]/src/husky/husky_description/urdf/realsense.urdf.xacro
```
Disable ekf localization by adding the following to bashrc:
```
export ENABLE_EKF=False
```

### Run
```
roslaunch husky_gazebo heightmap.launch
roslaunch husky_viz view_robot.launch
```

### Issues
* Texture not shown correctly
```bash
rm -rf ~/.gazebo/paging/
```

### Refs
[Gazebo: Heightmap Tutorial](https://vimeo.com/58409707)
