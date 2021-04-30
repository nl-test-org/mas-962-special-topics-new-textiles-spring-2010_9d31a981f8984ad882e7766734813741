---
course_id: mas-962-special-topics-new-textiles-spring-2010
layout: course_section
parent_title: 'Assignment 6: Networked Wearable'
title: 'Assignment 6: Hello U.S.A.!!'
type: course
uid: d9c642520aba741e8bc3ef40039896ca

---

| « Previous: [student work sample]({{< baseurl >}}/sections/assignments-and-projects/networked-wearable/assignment-6-wrist-based-way-finding) | Next: Return to [Assignment 6 description]({{< baseurl >}}/sections/assignments-and-projects/networked-wearable) » 

_By Yang Yang and three anonymous MIT students_  

![Schematic of United States map with grid of LEDs, controlled by circuits.](/courses/media-arts-and-sciences/mas-962-special-topics-new-textiles-spring-2010/assignments-and-projects/networked-wearable/assignment-6-hello-u.s.a./image002.gif)

Coordinate system that we used to light the LEDs from the LilyPad.

These Vertical pins were set to LOW: 11, 12, 13, a0(14), a1(15), a2(16), a3(17), a4(18), a5(19), 2, 3.  
These Horizontal pins were set to HIGH: 10, 9, 8, 7, 6, 5, 4.

Charlieplex State Drawing Detail
--------------------------------

We did not have enough pins on our LilyPad to control each led separately. Using charlieplexing we can have up to n/2\*(n/2) leds, where n is the number of pins on our Lilypad.

A grid of conductive fabric was made, positive legs of the LEDs were sewn to horizontal bars, the ground leg was sewn to the vertical strips.

We could then program the power to be sent to each LED, and turn all the others off by making them the opposite charge of the LED we wanted to light up.

The horizontal pins were set to HIGH and the vertical pins set to LOW. Each state had an associated LED, to turn on a particular pin its horzontal bar was called at HIGH and its vertical bar was called at LOW.

Wikipedia has a good reference article on [charlieplexing](http://en.wikipedia.org/wiki/Charlieplexing).

Charlieplexing  
 
------------------

![Photo of fabric with a grid pattern on it.](/courses/media-arts-and-sciences/mas-962-special-topics-new-textiles-spring-2010/assignments-and-projects/networked-wearable/assignment-6-hello-u.s.a./SewnLeds.jpg)

The back of the map. The LEDs are sewn positive leg to horizontal and ground to vertical. Felt pads are used to keep horizontal and vertical layers apart.  

![Photo of circular LilyPad device in some fabric, layed on top of grid-covered fabric.](/courses/media-arts-and-sciences/mas-962-special-topics-new-textiles-spring-2010/assignments-and-projects/networked-wearable/assignment-6-hello-u.s.a./Lillypadlayer.jpg)

The LilyPad layer set over the charlieplex felt layer. This is the final layer that has the conductive thread connecting from the LilyPad to the charlieplex grid at the edges of the felt.

| « Previous: [student work sample]({{< baseurl >}}/sections/assignments-and-projects/networked-wearable/assignment-6-wrist-based-way-finding) | Next: Return to [Assignment 6 description]({{< baseurl >}}/sections/assignments-and-projects/networked-wearable) »