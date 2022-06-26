# Fisheye Camera Sensors

This repository contains virtual sensors developed for a 200º fisheye camera. These were designed for use in a small ground robot with the camera mounted above and aimed downwards.
Each of the sensors can be used by launching the respective launch file, for example for the simulated lidar:
```
roslaunch fisheye_camera_simulated_sensors_ros1 simulated_lidar.launch
```

## Simulated LiDAR

This sensor simulates a Light Detection And Ranging sensor with 90 rays distributed evenly around the robot. It publishes LaserScan messages with relative values.

## Object Detection

This sensor improves upon the sensor presented in the [SERP project](https://github.com/jorgef1299/SERP), providing proximity values for obstacles in four positions: front, front-left, front-right and rear. It publishes custom ObjectDetection messages.

## Proximity Sensor

This sensor simulates a front mounted laser sensor with 5 rays distributed evenly over a 90º area in front of the robot. It publishes LaserScan messages with approximate values.
