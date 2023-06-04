---
title: "Coding Period Week 1"
categories:
  - Blog
permalink: /Coding-period-week1/
toc_label: Table of Content
toc: true
sidebar:
  nav: "docs"
---

In the weekly meet we did the sprint planning and listed out the issues to work on for the coming two weeks.\
[Sprint 1](https://github.com/orgs/JdeRobot/projects/2/views/1)
## Work Done
* Added and tested Aruco markers to Package Delivery exercise
* Created build.sh to ease building miniRADIs
* Restructured miniRADI dockerfiles to optimise build times
* Refactored and optimised the Humble Dockerfile

### Issues Created
* [https://github.com/JdeRobot/RoboticsAcademy/issues/2091](https://github.com/JdeRobot/RoboticsAcademy/issues/2091)
* [https://github.com/JdeRobot/RoboticsAcademy/issues/2088](https://github.com/JdeRobot/RoboticsAcademy/issues/2088)


### Issues Fixed
* [https://github.com/JdeRobot/RoboticsAcademy/issues/2091](https://github.com/JdeRobot/RoboticsAcademy/issues/2091)
* [https://github.com/JdeRobot/RoboticsInfrastructure/issues/280](https://github.com/JdeRobot/RoboticsInfrastructure/issues/280)

### PRs created
* [https://github.com/JdeRobot/drones/pull/190](https://github.com/JdeRobot/drones/pull/190)
* [https://github.com/JdeRobot/RoboticsAcademy/pull/2093](https://github.com/JdeRobot/RoboticsAcademy/pull/2093)
* [https://github.com/JdeRobot/RoboticsAcademy/pull/2094](https://github.com/JdeRobot/RoboticsAcademy/pull/2094)
* [https://github.com/JdeRobot/RoboticsAcademy/pull/2098](https://github.com/JdeRobot/RoboticsAcademy/pull/2098)
* [https://github.com/JdeRobot/RoboticsInfrastructure/pull/290](https://github.com/JdeRobot/RoboticsInfrastructure/pull/290)
* [https://github.com/JdeRobot/RoboticsAcademy/pull/2105](https://github.com/JdeRobot/RoboticsAcademy/pull/2105)

### Details of MRs
* Addition of Aruco markers of ID 0, 1 and 2 to reference multiple package destinations:
  ![alt]({{ site.url }}{{ site.baseurl }}/assets/images/Aruco_marker_Destinations.png)
  * Aruco Marker ID 0:

  ![alt]({{ site.url }}{{ site.baseurl }}/assets/images/Aruco_marker_0.png)

* Creation of build.sh with extended flags for RADI building:
  ![alt]({{ site.url }}{{ site.baseurl }}/assets/images/build_sh_help.png)

  ![alt]({{ site.url }}{{ site.baseurl }}/assets/images/build_sh_building.png)

* Optimised Humble base RADI: Decreased Humble base RADI size from 6.8 GBs to 5.3 GBs
  * Made code styling uniform, easier to read and extend
  * Removed packages like alsa-utils alsa-oss lxde-common (not needed)
  * Removed ros-humble-desktop, instead use ros-humble-ros-base (decreases the size)
  * Clubbed apt installs together to reduce the number of layers and decrease the size
  * Restructured Python dependency list and put it at the bottom, since these are likely to have additions in the future, having them at the bottom will help to use the Docker cache for system dependencies more effectively.
  * Removed duplicate pip installs

## Plan for next week

* Addition of PX4 to ROS2 humble Dockerfile
* Explore multi-distro RADIs
* Moving drone assets to RoboticsInfrastructure (Custom Robots)