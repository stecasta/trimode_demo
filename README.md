# Software for Trimode robot

## load gazebo model
roslaunch jackal_gazebo jackal_world.launch

## navigation w/o map
roslaunch jackal_navigation odom_navigation_demo.launch

roslaunch jackal_viz view_robot.launch config:=navigation

## making a map 
roslaunch jackal_navigation gmapping_demo.launch

roslaunch jackal_viz view_robot.launch config:=gmapping

## navigation with premade map 
roslaunch jackal_navigation amcl_demo.launch 

roslaunch jackal_viz view_robot.launch config:=localization
