---
course_id: mas-962-special-topics-new-textiles-spring-2010
layout: course_section
parent_title: 'Assignment 6: Networked Wearable'
title: 'Assignment 6: Wrist-based Way-finding'
type: course
uid: 77520b74548a605c22bd5f4919a9b598

---

| « Previous: Return to [Assignment 6 description]({{< baseurl >}}/sections/assignments-and-projects/networked-wearable) | Next: [student work sample](/courses/media-arts-and-sciences/mas-962-special-topics-new-textiles-spring-2010/assignments-and-projects/networked-wearable/assignment-6-hello-u.s.a.) » 

_New Textiles students: Dawn Wendell, Rizal Muslimin and anonymous student  
Communicating with Mobile Technologies students: Thomas Lipoma and anonymous MIT student_

![Close-up photo of several electronic devices sewn into a piece of fabric.](/courses/media-arts-and-sciences/mas-962-special-topics-new-textiles-spring-2010/assignments-and-projects/networked-wearable/assignment-6-wrist-based-way-finding/device01.jpg)

The wristband component of the way-finder.

For our collaboration with the Communicating with Mobile Technologies class, we decided to make a wearable information display with two RGB LEDs. We envisioned these LEDs being used for guidance similar to the kids games of "simon says" or "hot and cold", with the LEDs changing colors in response to the user's orientation and distance from a target location. This is a more passive way of giving directions, with the user having to be actively involved in the discovery of the target place.

The Textiles team built a wrist-based device, connected with the LilyPad and two RGB LEDs. We also completed the bluetooth connection from the phone to the device and troubleshot the system using the output from the phone compass.

![Collage of various design elements: Android mobile phone, wristband and several code excerpts.](/courses/media-arts-and-sciences/mas-962-special-topics-new-textiles-spring-2010/assignments-and-projects/networked-wearable/assignment-6-wrist-based-way-finding/wrist1.gif)

Design elements of the wrist-based way-finder.

{{< youtube 0zitghvkD5w >}}

Here is a video of the wristband responding to compass directions from the phone.

One LED changes color in response to the orientation of the phone, and the other LED changes from red to green when the phone has been held in the green ("correct") position for longer than 3 seconds. This pause / response is intended to signify that you have traveled in the correct direction and have now arrived at the destination.

![Diagram depicting two potential applications: navigation, shown by a bicyclist consulting an online map tool, and monitoring, shown by a runner communicating heart data to some medical devices.](/courses/media-arts-and-sciences/mas-962-special-topics-new-textiles-spring-2010/assignments-and-projects/networked-wearable/assignment-6-wrist-based-way-finding/wrist2.gif)

Potential applications include mobile navigation support and physiological monitoring. (Map image source © Google. All rights reserved. This content is excluded from our CreativeCommons license. For more information, see [/fairuse](/fairuse))

Lessons Learned
---------------

*   We tried to make our own circuit, but were not able to get it working. Should have tested the circuit before sewing it to the wristband.
*   The battery holder we were given gave us lots of trouble - the leads kept falling off so we spent a lot of time ripping them off the wristband and resoldering them, even though we tried to sew the leads in place for strain-relief.
*   It was very hard to do anything in parallel because we had one device, one LilyPad, one phone, and two groups from the Mobile Technologies class who both needed to use the textile device.
*   Scheduling undergrads and grads together is HARD. We were never able to actually meet up with our Mobile Technologies teammates.

![Photo of two people at a table working on the system: mobile phone, wristband, and laptop.](/courses/media-arts-and-sciences/mas-962-special-topics-new-textiles-spring-2010/assignments-and-projects/networked-wearable/assignment-6-wrist-based-way-finding/working02.jpg)

Testing the system.

Contributions
-------------

Anonymous student: software, phone connection  
Dawn: wristband, documentation  
Rizal: circuit, soldering, documentation

Code
----

BDR Standalone ([TXT](/courses/media-arts-and-sciences/mas-962-special-topics-new-textiles-spring-2010/assignments-and-projects/networked-wearable/assignment-6-wrist-based-way-finding/bdr_standalone_code.txt))  
BDR Integrated ([TXT](/courses/media-arts-and-sciences/mas-962-special-topics-new-textiles-spring-2010/assignments-and-projects/networked-wearable/assignment-6-wrist-based-way-finding/bdr_integrated_code.txt))

| « Previous: Return to [Assignment 6 description]({{< baseurl >}}/sections/assignments-and-projects/networked-wearable) | Next: [student work sample](/courses/media-arts-and-sciences/mas-962-special-topics-new-textiles-spring-2010/assignments-and-projects/networked-wearable/assignment-6-hello-u.s.a.) »