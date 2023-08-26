---
title: "Coding Period Week 12"
categories:
  - Blog
permalink: /Coding-period-week12/
toc_label: Table of Content
toc: true
sidebar:
  nav: "docs"
---

This week was focused on resolving bugs in Rescue People humble migration.

## Work Done
* Resolved issue with drone_dual_cam model not publishing camera feed
* Updated gazebo_ros_plugin in the iris model
* The boat model no longer sinks
* The drone is able to takeoff in the rescue world now
* Tested camera images in the gui 
* Fixed rosdep install failing
* moved CustomRobots in Docker image instead of copying to reduce container size

  ![alt]({{ site.url }}{{ site.baseurl }}/assets/images/rescue_people_ros2_gui_images.png)

## Issue pending
* Creating a HAL object in exercise.py clashes something with webserver - these can be ignored because the connection is made after a while
  ![alt]({{ site.url }}{{ site.baseurl }}/assets/images/HAL_issue.png)
* Sometimes the goal is rejected
* Sometimes the exercise thread is not terminated properly after quitting the exercise
* Camera images shown in the gui have the rate too low

### Issues Fixed
* [https://github.com/JdeRobot/RoboticsAcademy/issues/2223](https://github.com/JdeRobot/RoboticsAcademy/issues/2223) (under review)

### PRs created / worked on
* [https://github.com/JdeRobot/RoboticsAcademy/pull/2224](https://github.com/JdeRobot/RoboticsAcademy/pull/2224)
* [https://github.com/JdeRobot/RoboticsInfrastructure/pull/313](https://github.com/JdeRobot/RoboticsInfrastructure/pull/313)
* [https://github.com/JdeRobot/RoboticsAcademy/pull/2226](https://github.com/JdeRobot/RoboticsAcademy/pull/2226)
* [https://github.com/JdeRobot/RoboticsAcademy/pull/2225](https://github.com/JdeRobot/RoboticsAcademy/pull/2225)


## Plan for next week
* Update drone_wrapper to not use aerostack behaviours
* Fix the drone images rate issue
