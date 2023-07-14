<h1 align="center">Project #2 for Udacity's Robotics Nanodegree - Go Chase It</h1>

[image1]: img1.png "img1"
![alt text][image1]

## Introduction
This is a project for Udacity's Robotics NanoDegree. It's a simulated world built in Gazebo that includes a building, a robot, and a plugin.

## Concepts and Classes
Concepts explored in this project:

  - Gazebo model and world-building
  - Gazebo Plugins
  - C++

## Getting Started
To view this project, you must have Gazebo installed on Linux.

Following Instructions:

[Gazebo download and installation instructions](http://gazebosim.org).

With Gazebo installed, download/clone the repository and copy the ```model``` , ```script``` and ```world``` directories into the workspace directory:

```bash
$ mkdir workspace
$ cd workspace
$ git clone https://github.com/bmaxdk/RoboticsND-Build-My-World.git
$ cp -R RoboticsND-Build-My-World/model RoboticsND-Build-My-World/script RoboticsND-Build-My-World/world .
$ rm -rf RoboticsND-Build-My-World.
```

You first must build the plugin, so create a build folder and navigate to it:

```bash
$ mkdir build && cd build
```
Then build the plugin:

```bash
$ cmake .. && make
```

And update the GAZEBO_PLUGIN_PATH environment variable:

```bash
$ export GAZEBO_PLUGIN_PATH=${GAZEBO_PLUGIN_PATH}:${PWD}
```

Once the plugin is built, open the world in Gazebo:

```bash
$ gazebo ../world/robotl1.world
```

Once it launch you will see welcome message `Welcome to Hyunjin's World!`

