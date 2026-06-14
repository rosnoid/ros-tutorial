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
$ ros2 topic info /turtle1/cmd_vel

```
