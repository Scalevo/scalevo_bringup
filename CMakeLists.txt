cmake_minimum_required(VERSION 2.8.3)
project(scalevo_bringup)

find_package(catkin REQUIRED COMPONENTS roslaunch)

catkin_package()

roslaunch_add_file_check(launch)

install(PROGRAMS scripts/install 
   DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION})


