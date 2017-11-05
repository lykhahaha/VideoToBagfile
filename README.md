# Avi to rosbag file in ROS

A simple description of converting video files to ROS bagfiles.

## video to bagfile

1. we need to install [ROS Kinetic](http://wiki.ros.org/kinetic/Installation/Ubuntu) on Ubuntu.
2. use catkin or any build system.
3. Download [video_stream_opencv](https://github.com/ros-drivers/video_stream_opencv). Go to the launch folder of [video_stream_opencv](https://github.com/ros-drivers/video_stream_opencv) and open video_file.launch. Then, add the avi file path to the value section of "video_stream_provider".
4. build [video_stream_opencv](https://github.com/ros-drivers/video_stream_opencv) to run a node to show your avi file.
5. In a new terminal, run roscore. Then, run this command: roslaunch video_stream_opencv video_file.launch 
6. open a new terminal, run this command: rosbag record -O filename /videofile/image_raw

 
