---
title: "Coding Period Week 13"
categories:
  - Blog
permalink: /Coding-period-week13/
toc_label: Table of Content
toc: true
sidebar:
  nav: "docs"
---

This week was focused on testing the migration and investigating/resolving issues found.

## Work Done
* Began work to replace Aerostack behaviours (takeoff and landing) with simpler API calls
* Worked on the issue with Aerostack unable to fetch transforms from the past, work it around by using system time.
  ![alt]({{ site.url }}{{ site.baseurl }}/assets/images/as2_transforms_issue.png)
* Another issue was with the drone state not updating when not using behaviours, was resolved by making a ros2 service call.
* Investigated on intermittent drone take off failures in rescue people world.
* Tried to use threading in drone_wrapper.py to resolve the lag in GUI images.
* Resolved issue with the Web console not printing debug messages of user's code.

## Issue pending
* Landing still uses Aerostack behaviour.
* Drone takeoff is rejected intermittently.
* Camera images shown in the gui have the rate too low

### Issues Fixed
* [https://github.com/JdeRobot/RoboticsAcademy/issues/2223](https://github.com/JdeRobot/RoboticsAcademy/issues/2223) (under review)
* [https://github.com/JdeRobot/RoboticsAcademy/issues/2227](https://github.com/JdeRobot/RoboticsAcademy/issues/2227)
* [https://github.com/JdeRobot/RoboticsInfrastructure/issues/314](https://github.com/JdeRobot/RoboticsInfrastructure/issues/314) (in progress)

### PRs created / worked on
* [https://github.com/JdeRobot/RoboticsAcademy/pull/2228](https://github.com/JdeRobot/RoboticsAcademy/pull/2228)
* [https://github.com/JdeRobot/RoboticsInfrastructure/pull/316](https://github.com/JdeRobot/RoboticsInfrastructure/pull/316)


## Plan for next week
* Update landing code to not use behaviours
* Fix the drone images rate issue
* Investigate on drone takeoff failures
* Wrap up the project
