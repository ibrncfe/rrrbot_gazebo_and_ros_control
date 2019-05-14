This package is related to ros_control library for a robotic arm connected with camera. this example is created by https://github.com/JoshMarino/gazebo_and_ros_control.git some changes were made now by adding some missing files.

if you are running ros on Linux/VmWare so you need to run this command
export LIBGL_ALWAYS_SOFTWARE=1

Quick Guide to run:

first step:
roslaunch rrrbot_files rrrbot_launch.launch



Second Step:
rostopic pub /rbot/joint3_position_controller/command std_msgs/Float64 "data: 1" 
for manual control

third Step:
rosrun rrrbot_files rrrbot_position_controller.py 

