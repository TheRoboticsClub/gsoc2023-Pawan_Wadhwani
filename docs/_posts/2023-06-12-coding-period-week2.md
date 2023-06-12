---
title: "Coding Period Week 2"
categories:
  - Blog
permalink: /Coding-period-week2/
toc_label: Table of Content
toc: true
sidebar:
  nav: "docs"
---

In the weekly meet we did the sprint planning and listed out the issues to work on for the coming two weeks.\
[Sprint 1](https://github.com/orgs/JdeRobot/projects/2/views/1)
## Work Done
* Installed and tested PX4 Autopilot v1.14 beta2 locally on ROS2
* Added PX4 Autopilot to Humble Dockerfiles
* Discovered that Gazebo11 is no longer being installed correctly with current gpg key
* Moved Drone assets to RoboticsInfrastructure Repo

### Issues Created
* [https://github.com/JdeRobot/RoboticsAcademy/issues/2118](https://github.com/JdeRobot/RoboticsAcademy/issues/2118)

### Issues Fixed
* [https://github.com/JdeRobot/RoboticsInfrastructure/issues/221](https://github.com/JdeRobot/RoboticsInfrastructure/issues/221)
* [https://github.com/JdeRobot/RoboticsInfrastructure/issues/278](https://github.com/JdeRobot/RoboticsInfrastructure/issues/278)
* [https://github.com/JdeRobot/RoboticsInfrastructure/issues/280](https://github.com/JdeRobot/RoboticsInfrastructure/issues/280)

### PRs created

* [https://github.com/JdeRobot/RoboticsInfrastructure/pull/297](https://github.com/JdeRobot/RoboticsInfrastructure/pull/297)
* [https://github.com/JdeRobot/RoboticsAcademy/pull/2119](https://github.com/JdeRobot/RoboticsAcademy/pull/2119)

### Details of MRs
* The major target of this week was to make a drone takeoff on ROS2 with PX4, which was accomplished.
    ![alt]({{ site.url }}{{ site.baseurl }}/assets/images/drone_takeoff.png)

* Added the required setup for PX4-Autopilot to ROS2 Dockerfiles:
  * Added system and pip Dependencies
  * Added PX4 Autopilot
  * Added MicroXRCE-DDS-Agent
  * Removed redundant packages

## Plan for next week

* Explore multi-distro RADIs
