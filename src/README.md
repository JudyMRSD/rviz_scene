ros/AR_tag
-------------
TF
roslaunch apriltags apriltags_view.launch
//roslaunch apriltags apriltags.launch
roslaunch kinect2_bridge kinect2_bridge.launch
rostopic echo /apriltags/detections

rosrun rviz rviz
//rosrun tf static_transform_publisher 0 0 0 0 0 0 1 world map 1

rosrun apriltags apriltag_kinect_tf





---------------------------
-----------------------------
ros/rviz_scene

catkin_make
. ./devel/setup.bash
cd to /home/jin/ros/rviz_scene/src/urdf_tutorial

------------------
roslaunch urdf_tutorial display.launch model:=urdf/bin.urdf

rosrun tf static_transform_publisher 0 0 0 0 0 0 1 world base_link 1

----------------
to view tf tree in pdf:

rosrun tf view_frames
--------------
screenshot and tf tree  is in result folder

-----------------





