---
title: "Sitting Desktop Garden"
summary: "A customisable pot plant for the home office desk that tracks your posture"
date: "2024-10-18"
tags: ["machine learning"]
readTime: true
---

![Sitting Desktop Garden Prototype](/projects/sitting-desktop-garden/prototype.png "Sitting Desktop Garden prototype. (1): plant raising mechanism, (2): posture-tracking camera, (3): OLED display, (4): buttons for interacting with the display.")

The Sitting Desktop Garden (SDG) is a cute and customisable artificial potted plant for the home office desk. It monitors the user's posture, providing gentle reminders and gamified incentives to maintain a healthy sitting position as you work. Reminders are delivered through haptic feedback in a vibrating mousepad, which is non-intrusive to the user's workflow, and demonstrating consistently good posture unlocks more beautiful plant growth.

The SDG is controlled with a Raspberry Pi, which runs all machine learning models and stores all user data locally. No internet connection is required once the Raspberry Pi is set up.

We use a facial recognition system to facilitate user logins and registrations to allow for multiple users to share one SDG. This can be useful in shared workspaces and offices (hot desking). Once the user is logged in, the camera monitors user posture by tracking their body landmarks and determining their neck and hip angles.

Real-time feedback is delivered via a vibrating mousepad, which reminds the user to sit up straight if they are not sitting correctly. Current-session feedback can be viewed via the SDG's monitor to show the user how their posture has progressed over the current session, as well as via the physical growth of the potted plant.

This is a [DECO3801](https://programs-courses.uq.edu.au/course.html?course_code=deco3801) group project that I worked on in 2024 Semester 2.

---

* <a href="https://github.com/LimaoC/sitting-desktop-garden/" target="_blank">GitHub</a>
