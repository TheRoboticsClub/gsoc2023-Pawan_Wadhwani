---
title: "Coding Period Week 5 and 6"
categories:
  - Blog
permalink: /Coding-period-week5-and-6/
toc_label: Table of Content
toc: true
sidebar:
  nav: "docs"
---

These couple of weeks were focused on getting experience with Aerostack, exploring ros launch options, and RAM launchers working.

Sprint Board
![alt]({{ site.url }}{{ site.baseurl }}/assets/images/sprint3-end.png)

## Work Done
* Aerostack install in Docker merged
* Unifying RAM launchers merged
* Explored ROS2 launch options without using python subprocess, The idea was rejected ([Details](https://github.com/orgs/JdeRobot/projects/2/views/1?pane=issue&itemId=31890813))
* Able to run Aerostack in a docker image on browser using VNC [Source](https://github.com/aerostack2/aerostack2/pull/294)
  - ![alt]({{ site.url }}{{ site.baseurl }}/assets/images/aerostack.png)
* Unified sourcing of ROS2 workspaces in .bashrc
* Resolved Pydantic error
* Worked on ROS2 RAM setting Environment variables on runtime (in progress)

### Issues Created
* [https://github.com/JdeRobot/RoboticsAcademy/issues/2163](https://github.com/JdeRobot/RoboticsAcademy/issues/2163)
* [https://github.com/JdeRobot/RoboticsApplicationManager/issues/45](https://github.com/JdeRobot/RoboticsApplicationManager/issues/45)

### Issues Fixed
* [https://github.com/JdeRobot/RoboticsApplicationManager/issues/45](https://github.com/JdeRobot/RoboticsApplicationManager/issues/45)
* [https://github.com/JdeRobot/RoboticsAcademy/issues/2166](https://github.com/JdeRobot/RoboticsAcademy/issues/2166)

### PRs created / worked on
* [https://github.com/JdeRobot/RoboticsAcademy/pull/2165](https://github.com/JdeRobot/RoboticsAcademy/pull/2165)
* [https://github.com/JdeRobot/RoboticsAcademy/pull/2162](https://github.com/JdeRobot/RoboticsAcademy/pull/2162)
* [https://github.com/JdeRobot/RoboticsAcademy/pull/2161](https://github.com/JdeRobot/RoboticsAcademy/pull/2161)
* [https://github.com/JdeRobot/RoboticsAcademy/pull/2153](https://github.com/JdeRobot/RoboticsAcademy/pull/2153)

## Plan for next week

* Creating Aerostack Launcher in RAM
* Migration of Rescue People exercise
