---
title: "Coding Period Week 7"
categories:
  - Blog
permalink: /Coding-period-week7/
toc_label: Table of Content
toc: true
sidebar:
  nav: "docs"
---

This week was focused on exploring Aerostack and debugging the Rescue People RR drone exercise, It had PX4 failing to launch correctly. as well as whether we need set_environment during runtime. Having hooks in Custom Robots does the same work, this can help in reducing the complexity of the database file since we can remove resource_folders,model_folders and plugin_folders.

## Work Done
* Tested and Debugged the aerostack2 launch file on ign gazebo in a docker environment
* Ran Rescue People RR exercises
* Tested the need for set_environment during runtime vs setting it using hooks by the Custom Robots package

### Issues Fixed
* [https://github.com/JdeRobot/RoboticsApplicationManager/issues/50](https://github.com/JdeRobot/RoboticsApplicationManager/issues/50)

### PRs created / worked on
* [https://github.com/JdeRobot/RoboticsApplicationManager/pull/55](https://github.com/JdeRobot/RoboticsApplicationManager/pull/55)
* [https://github.com/JdeRobot/RoboticsInfrastructure/pull/307](https://github.com/JdeRobot/RoboticsInfrastructure/pull/307)

## Plan for next week

* Creation of ROS2 drones package
