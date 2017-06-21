## PointCloud (PC)
+ Derived from Hessian
+ src/IOWrapper/Pangolin/KeyFrameDisplay.cpp#drawPC(...) and src/IOWrapper/Pangolin/KeyFrameDisplay.cpp#refreshPC(...) 
is where this occurs in Pangolin
+ Should be something similar in the sample OutputIOWrapper
+ Will need to create a similar wrapper and shave the points into a pcl::PointCloud<T> or sensor_msgs/PountCloud2 object
