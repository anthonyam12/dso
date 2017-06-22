## PointCloud (PC)
+ Derived from Hessian
+ src/IOWrapper/Pangolin/KeyFrameDisplay.cpp#drawPC(...) and src/IOWrapper/Pangolin/KeyFrameDisplay.cpp#refreshPC(...) 
is where this occurs in Pangolin
+ Should be something similar in the sample OutputIOWrapper
+ Will need to create a similar wrapper and shave the points into a pcl::PointCloud<T> or sensor_msgs/PountCloud2 object
### Resources 
+ http://www.pcl-users.org/pcl-PointCloud-lt-T-gt-vs-sensor-msgs-PointCloud2-td2983165.html
+ http://docs.ros.org/api/sensor_msgs/html/msg/PointCloud2.html
+ http://docs.pointclouds.org/1.7.1/classpcl_1_1_point_cloud.html


## Modifcations
To test different IOWrappers they will need to be registered. Alternatively, just make a backup of the sample wrapper in src/IOWrapper/OutputWrapper/SampleOutputWrapper.h and modify this wrapper as need be, since it's already registered. 

To build the changes just run `make -j <# jobs>' in the CMake build directory.
