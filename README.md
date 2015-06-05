# scalevo_bringup
 
 clone scalevo_bringup to computer

autostart depends on robot_upstart plugin

    https://github.com/clearpathrobotics/robot_upstart 

Achtung: indingo branch

create install directory in catkin workspace

build workspace

    rosrun robot_upstart install scalevo_bringup/launch/scalevo.launch

autostart depends also on daemontools

    sudo apt-get install daemontools 

reboot computer and roscore & launch file will start in background

see console output with

    sudo tail /var/log/upstart/scalevo.log -n 30

start & stop service that is called on start up manually with 

    sudo service scalevo start
    sudo service scalevo stop

