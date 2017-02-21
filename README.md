This [ROS] stack provides a real-time 2D and 3D [ICP]-based SLAM system that
can fit a large variety of robots and application scenarios, without any code
change or recompilation.

Information about this stack, including installation and compilation, is available on the [ROS] wiki at [http://www.ros.org/wiki/ethzasl_icp_mapping](http://www.ros.org/wiki/ethzasl_icp_mapping).

[ROS]: http://www.ros.org
[ICP]: http://en.wikipedia.org/wiki/Iterative_Closest_Point

Compile for Kinetic 

```
mkdir -p catkin_ws/ws1/src
cd catkin/ws1/src
catkin_init_workspace
git clone https://github.com/ethz-asl/libnabo.git
git clone https://github.com/ethz-asl/libpointmatcher.git
cd ..
catkin_make_isolated
source devel_isolated/setup.bash

cd ..
mkdir -p ws2/src
cd ws2/src
clone this source
git checkout kinetic
cd ..
catkin_make

```


