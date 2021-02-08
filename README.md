# ur5e_egp_moveit_config
Moveit config folder for the UR5e + EGP50 gripper

## Start only with rviz
* `roslaunch ur5e_egp50_moveit_config demo_pick_place.launch rviz:=true`
  
## Start with real robot:
* `roslaunch ur_robot_driver ur5e_bringup.launch robot_ip:=192.168.56.1 \
  kinematics_config:=$(rospack find ur5e_egp50_moveit_config)/config/ur5e_calibration.yaml`
* `roslaunch ur5e_egp50_moveit_config ur5e_egp50_moveit_planning_execution.launch sim:=false rviz:=true`