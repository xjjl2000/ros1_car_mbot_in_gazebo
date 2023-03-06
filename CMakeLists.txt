cmake_minimum_required(VERSION 2.8.3)
project(car_mbot)

find_package(catkin REQUIRED
    roscpp
    rospy
    std_msgs
)

catkin_package()

include_directories(
  ${catkin_INCLUDE_DIRS}
)

install(DIRECTORY launch
  DESTINATION share/${CATKIN_PACKAGE_SHARE_DESTINATION})

install(DIRECTORY worlds
  DESTINATION share/${CATKIN_PACKAGE_SHARE_DESTINATION})

install(DIRECTORY urdf
  DESTINATION share/${CATKIN_PACKAGE_SHARE_DESTINATION})  

install(DIRECTORY meshes
  DESTINATION share/${CATKIN_PACKAGE_SHARE_DESTINATION})  
