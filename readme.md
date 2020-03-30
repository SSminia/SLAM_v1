# Pepe Slam
### ROS navigation simulation by Sean Sminia and Ray Mindiola


##### Imporant
.dae files inside the world file have hardcoded path names. these need to set locally to run the navigation

### Setup
1. Follow marian tutorial on github (https://github.com/marckri/ROS-Helper/blob/master/doc/turtlebot3-sim.md)
2. Create new package
3. Copied default gazebo launchfile into package
4. Download world files from (https://github.com/hussamayoub/turtlebot3melodic.git)
5. Added world files to package
6. Edited simulation file with launch files
7. Mapping file based on suii (https://github.com/RoboHubEindhoven/suii/tree/master/suii_bringup/launch)
8. Navigation file based on suii, modified values to adjust the different robot type
9. The map was done manually, moving the robot around using teleop_twist_joy

### Coding and tweaking
10. Nagivate and tweak navigation variables with Rviz and rqt
11. use example python to set goal using movebase
12. create python script to loop between goals, values harded coded in the script itself
 
### How to launch
rosboot in all terminals
new terminal launch SLAM_v1 turtleSim.launch
new terminal launch SLAM_v1 navigation.launch
new terminal rviz, 2d pos estimate
new terminal rosrun SLAM_v1 pepe.py
