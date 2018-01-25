# x_arm

## to run x_arm in gazebo

> rosrun x_arm_description x_arm_world.launch
 
## To view RGB raw image

> rosrun image_view image_view image:=/rgbd_camera/rgb/image_raw

## To view IR image

> rosrun image_view image_view image:=/rgbd_camera/ir/image_raw

## To view depth image

> rosrun image_view image_view image:=/rgbd_camera/depth/image_raw

## also view in rviz (add pointCloud 2)

> rosrun rviz rviz -f /rgbd_camera_optical_frame

## run gazebo with ros_control 

> roslaunch x_arm_gazebo x_arm_gazebo_control.launch

## Move joints

> rostopic pub /x_arm/joint2_position_controller/command std_msgs/Float64 "data: 1.0" 
