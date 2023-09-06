---
title: "Coding Period Final Week"
categories:
  - Blog
permalink: /Coding-period-week14/
toc_label: Table of Content
toc: true
sidebar:
  nav: "docs"
---

The final week was focused on wrapping up things and merging any pending MRs. I also made the result video and uploaded it on the JdeRobot youtube channel

## Work Done
* Resolved issue with lag in drone images in the GUI by making a separate node to subscribe image topics.
* Resolved the intermittent drone take off issue by making the boat_beacon model's collision properties more stable by
  * Increasing friction
  * Decreasing bounce
  * Softer contacts and damping
* Completely replaced Aerostack behaviours (Takeoff and Landing) with simpler API calls, this makes running the exercise less computationally expensive.
* Fixed running PX4 and gzserver headlessly in Aerostack repository.
* Edited and uploaded the final video on youtube.

{% include video id="O8atiuEamp4" provider="youtube" %}

### PRs created / worked on
* [https://github.com/JdeRobot/RoboticsInfrastructure/pull/317](https://github.com/JdeRobot/RoboticsInfrastructure/pull/317)
* [https://github.com/JdeRobot/RoboticsInfrastructure/pull/318](https://github.com/JdeRobot/RoboticsInfrastructure/pull/318)
* [https://github.com/JdeRobot/RoboticsInfrastructure/pull/316](https://github.com/JdeRobot/RoboticsInfrastructure/pull/316)
* [https://github.com/aerostack2/aerostack2/pull/323](https://github.com/aerostack2/aerostack2/pull/323)


## Conclusion

I am pleased to announce that the core of the project has been successfully completed, with only minor issues remaining. As I transition into a more permanent role within the organization, I am committed to addressing these remaining challenges and ensuring the project's continued success. My GSoC experience has not only been a fulfilling journey but also marks the beginning of my long-term contribution to the organization and its mission. I am eager to build upon the foundation we've established and look forward to future collaborations with the team.

Beyond the technical aspects, GSoC has also taught me important soft skills such as effective communication, project management, and teamwork. These skills are crucial in any professional setting and will undoubtedly benefit me in my future endeavors.

In closing, Google Summer of Code has been a remarkable chapter in my journey as a developer, and I am excited to see where the future leads, armed with the skills, experiences, and connections I've gained during this unforgettable summer.