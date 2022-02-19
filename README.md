# usb_cam

ls /dev/video*

sudo apt install v4l-utils

v4l2-ctl -d /dev/video0 --list-formats-ext

http://wiki.ros.org/melodic/Installation/Ubuntu

sudo apt install ros-melodic-usb-cam 

cd catkin_ws/src/

git clone https://github.com/bosch-ros-pkg/usb_cam.git

cd ..

catkin_make


usb_cam-test.launch edit===>  /dev/video0, image_width"와 "image_height

usb_cam_node.cpp ====> /dev/video0, image_width"와 "image_height

**1920x1080

**60fps

**yuyv

source devel/setup.bash


roscore 

rosrun usb_cam usb_cam_node

rviz 
