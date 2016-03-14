0. Install packages:
https://github.com/meyerj/sbpl_lattice_planner/tree/indigo-devel
https://github.com/trainman419/dagny_nav.git

Change footprint_layer to  costmap_2d::VoxelLayer:
- /dagny_nav/dagny_nav_launch/global_costmap.yaml
- /dagny_nav/dagny_nav_launch/local_costmap.yaml to voxel layer

1. roslaunch golfcart_gazebo golfcart.launch 

2. rosrun golfcart_gazebo odom_transformation_node

3. rosrun golfcart_gazebo cmd_vel_to_ackermann_drive.py 

4. roslaunch dagny_nav_launch dagny_nav_gmapping.launch 
