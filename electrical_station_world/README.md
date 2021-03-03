# robotnik_station_world

**Description:** this package contain a world for Gazebo embedded in a ROS package, so you don't need set the gazebo path or do other configurations. 

<img src="img/station.png" width="90%">

Electrical substation located in station, Cantabria, Spain.

## General installation

In your workspace, clone the repository

```
$ git clone https://github.com/robert-ros/robotnik_station_world
```

Build the workspace and source it:

```
$ catkin build
$ source devel/setup.bash
```

Launch the package, you will see the  electrical substation

```
roslaunch robotnik_station_world station_world.launch 
```


## Use this map with your robot

In the workspace of your robot, clone this repository

```
$ git clone https://github.com/robert-ros/robotnik_station_world
```

Build the workspace and source it

```
$ catkin build
$ source devel/setup.bash
```

Launch you robot as always, but introduce the name of the world, in this case ```station_electrical_station.world```.

For example if you robot is a ```summit_xl``` working in ```melodic-devel``` branch, you musto to do:

```
$ roslaunch summit_xl_sim_bringup summit_xl_complete.launch gazebo_world:=station_electrical_station.world
```

 