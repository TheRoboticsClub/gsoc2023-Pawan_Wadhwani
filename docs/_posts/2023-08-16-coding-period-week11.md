---
title: "Coding Period Week 11"
categories:
  - Blog
permalink: /Coding-period-week11/
toc_label: Table of Content
toc: true
sidebar:
  nav: "docs"
---

This week was focused on finalising and streamlining the process flow and of launching of drone exercises and updating the package structure of jderobot_drones, along with this several bugs were solved.

## Work Done
* Testing the migration of rescue people exercise
* Updated jderobot_drones and got it merged
* Tested and merged combined Ilauncher for Aerostack and PX4
* Moved to run_sitl.sh script to lauch px4 from the previously made px4.launch.py
* Updated aerostack launch file to run microXRCE
* Solved issue in running run_sitl(launches gzserver and PX4) headlessly

![alt]({{ site.url }}{{ site.baseurl }}/assets/images/rescue_people_humble.png)

![alt]({{ site.url }}{{ site.baseurl }}/assets/images/rescue_people_drone_takeoff_ros2.png)

## Issue pending
* Drone model (iris_dual_cam) isn't publishing camera feed.
* Creating a HAL object in exercise.py clashes something with webserver
  ![alt]({{ site.url }}{{ site.baseurl }}/assets/images/HAL_issue.png)
* Issue with Rescue people world file that causes:
  * The boat model to sink 
  * The drone to not takeoff


### Issues Fixed
* [https://github.com/JdeRobot/RoboticsAcademy/issues/2223](https://github.com/JdeRobot/RoboticsAcademy/issues/2223) (In Progress)
* [https://github.com/JdeRobot/RoboticsApplicationManager/issues/72](https://github.com/JdeRobot/RoboticsApplicationManager/issues/72) (Finished)

### PRs created / worked on
* [https://github.com/JdeRobot/RoboticsApplicationManager/pull/73](https://github.com/JdeRobot/RoboticsApplicationManager/pull/73)
* [https://github.com/JdeRobot/RoboticsInfrastructure/pull/312](https://github.com/JdeRobot/RoboticsInfrastructure/pull/312)
* [https://github.com/JdeRobot/RoboticsAcademy/pull/2212](https://github.com/JdeRobot/RoboticsAcademy/pull/2212)
* [https://github.com/JdeRobot/RoboticsAcademy/pull/2224](https://github.com/JdeRobot/RoboticsAcademy/pull/2224)  
  (In Progress)


## Plan for next week

* Finish migration of Rescue People exercise
