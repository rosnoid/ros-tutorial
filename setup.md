# enable ros2 command for all your terminal
```
echo "source /opt/ros/lyrical/setup.bash" >> ~/.bashrc
source ~/.bashrc
```

# basic commands
```
$ ros2 node list
$ ros2 topic list
$ ros2 service list
$ ros2 action list
```

# turtle example
```
$ ros2 run turtlesim turtlesim_node
$ ros2 run turtlesim turtle_teleop_key

```

# topic
```
$ ros2 topic list
$ ros2 topic echo /turtle1/cmd_vel
$ ros2 topic info /turtle1/cmd_vel --verbose

$ ros2 topic hz /turtle1/pose  # view message rate
$ ros2 topic bw /turtle1/pose  # view message bandwidth

$ ros2 topic pub /turtle1/cmd_vel geometry_msgs/msg/Twist "{linear: {x: 2.0, y: 0.0, z: 0.0}, angular: {x: 0.0, y: 0.0, z: 1.8}}"   # publish message to a topic
```

# service
```
# /kill service name
# turtlesim_msgs/srv/Kill  request/response schema
# "{name: 'turtle1'}" service name
$ ros2 service call /kill turtlesim_msgs/srv/Kill "{name: 'turtle1'}"  
```


# params
```
$ ros2 param list #namespace followed by params
$ ros2 param get /turtlesim background_g
$ ros2 param set /turtlesim background_r 150

```





