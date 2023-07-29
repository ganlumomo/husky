husky_gazebo
=====

### Installation & Run
```bash
sudo cp -r models/heightmap/ /usr/share/gazebo-11/models/
roslaunch husky_gazebo heightmap.launch
```

### Issues
* Texture not shown correctly
```bash
rm -rf ~/.gazebo/paging/
```

### Refs
[Gazebo: Heightmap Tutorial](https://vimeo.com/58409707)
