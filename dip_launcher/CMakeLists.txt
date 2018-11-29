cmake_minimum_required(VERSION 3.0)
project(dip_launcher)

find_package(catkin REQUIRED COMPONENTS
  camera_to_inertial_conv
  pv_estimator
)

install(DIRECTORY launch/
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}/launch
  PATTERN ".svn" EXCLUDE
)
