mkdir -p ~/ros2_canopen_ws/src
cd ~/ros2_canopen_ws/src
git clone -b humble git@github.com:nicklgw/ros2_canopen.git 

nick@nick-evoc:~/ros2_canopen_ws$ ros2 launch canopen_tests robot_control_setup.launch.py

一柱擎天直立 joint1保持0°
ros2 topic pub /forward_position_controller/commands std_msgs/msg/Float64MultiArray '{"data":[0.0]}'
转一个角度 joint1转30°
ros2 topic pub /forward_position_controller/commands std_msgs/msg/Float64MultiArray '{"data":[0.52]}'
