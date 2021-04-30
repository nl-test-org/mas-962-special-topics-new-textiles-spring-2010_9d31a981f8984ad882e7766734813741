---
course_id: mas-962-special-topics-new-textiles-spring-2010
layout: course_section
parent_title: 'Assignment 3: "Hello World" Fabric PCBs, Part 2'
title: 'Assignment 3: PCButterfly'
type: course
uid: 1805af5becab6b007d48946d9bb9cafe

---

| « Previous: [student work sample]({{< baseurl >}}/sections/assignments-and-projects/fabric-pcbs-part-2/fractal-tree-bag) | Next: Return to [Assignment 3 description]({{< baseurl >}}/sections/assignments-and-projects/fabric-pcbs-part-2) » 

_By Xiao Xiao and two anonymous MIT students_

![Photo of a fabric butterfly with several LEDs on its wings, perched on a person’s hand.](/courses/media-arts-and-sciences/mas-962-special-topics-new-textiles-spring-2010/assignments-and-projects/fabric-pcbs-part-2/assignment-3-pcbutterfly/butterfly1.jpg)

The PCButterfly

The Concept
-----------

Our design is a light sensitive butterfly that turns on when in the dark. It can be easily incorporated onto clothing, bags, hair accessories etc. Our switch is a phototransistor located on the body of the butterfly design. Since the phototransistor is sensitive to changes in light it can be activated by shining and then removing the light source, yet will remain inactive in ambient light conditions.

The ATtiny13 microcontroller, has 4 pins available to connect to LEDs. Two allowed for pulse width modulation (PWM) so we decided to make the layout of the LEDs symmetrical with a pair that fade on and off on the upper wings, and ones that are steady on the lower wings.

The Design
----------

![Photo of circuit built in a breadboard, with many wires and clips coming out of it.](/courses/media-arts-and-sciences/mas-962-special-topics-new-textiles-spring-2010/assignments-and-projects/fabric-pcbs-part-2/assignment-3-pcbutterfly/butterfly_boardtest.jpg)

We first tested the layout on a breadboard before designing the actual butterfly circuit pattern.

![Hand-drawn circuit diagram with microcontroller in the center and several LEDs on leads.](/courses/media-arts-and-sciences/mas-962-special-topics-new-textiles-spring-2010/assignments-and-projects/fabric-pcbs-part-2/assignment-3-pcbutterfly/butterfly_circdiag.jpg)

The circuit diagram shows the phototransistor at B3, and LEDs connected at B0, B1(PWM lights) B2, B4 (non-PWM) B5 is for reset and is unconnected.

Our code ([TXT](/courses/media-arts-and-sciences/mas-962-special-topics-new-textiles-spring-2010/assignments-and-projects/fabric-pcbs-part-2/assignment-3-pcbutterfly/butterfly_code.txt))

There are two main fabric layers – a bottom layer for the main conductive area of the circuit, and the top layer that supports the ground wire, phototransistor, LEDs and resistors. The design incorporates iron-on adhesive conductive fabric as the substrate for the circuit. The phototransistor, LEDs and resistors are through components that source power through the microcontroller located at the center of the butterfly layout. A wire frame serves as an easily accessible ground wire as well as a structural support, which can be positioned to give the butterfly a more realistic shape.

![Photo showing top surface of the PCButterfly, with LEDs, integrated circuit device, ground wire and phototransistor.](/courses/media-arts-and-sciences/mas-962-special-topics-new-textiles-spring-2010/assignments-and-projects/fabric-pcbs-part-2/assignment-3-pcbutterfly/butterfly.jpg)

Top view of the PCButterfly.

An overall (cutting schematic) was rendered with Adobe Illustrator. A different image layer represents each fabric. Before cutting, it is necessary to separate the layers into discrete files in a format that can be imported to the laser cutter (ai v. 7, .dmx). Silicone molds were also created to add epoxy coatings to protect the soldered connections on the underside of the structure.

![Line drawing of the PCButterfly for use in controlling the laser cutter. ](/courses/media-arts-and-sciences/mas-962-special-topics-new-textiles-spring-2010/assignments-and-projects/fabric-pcbs-part-2/assignment-3-pcbutterfly/butterfly_layout.jpg)

Laser cutter schematic.

This video shows the laser cutter scoring our circuit. It is important to cut with the paper side up - so you may have to make a reflection of your design.

{{< youtube ggoWaPc_2xo >}}

PCButterfly laser cutter fabrication

The Fabrics
-----------

We tested a variety of fabrics including denim, leather and lightweight lining material. We wanted to be able to incorporate a range of textures into our design and allow for easy customization by simply rearranging the materials. The lining fabric was a bit too light to use on its own reliably, although we would like to experiment more with light fabrics in the future. The laser cutter was an ideal tool for creating decorative cutout designs on the wings. Both the denim and leather provided a robust structure for our PCB and our final design included a leather underside (most of the conductive fabric was adhered to this layer), lining fabric middle layer, and a denim top layer (ground wire frame, LEDs and resistors on this side).

![Photo of the leather underside of the PCButterfly, showing some stripes of silver conductive fabric. ](/courses/media-arts-and-sciences/mas-962-special-topics-new-textiles-spring-2010/assignments-and-projects/fabric-pcbs-part-2/assignment-3-pcbutterfly/butterfly_back.jpg)

Leather underside, with most of the conductive fabric.

![Photo of the PCButterfly in dim background light, with LEDs lit up. ](/courses/media-arts-and-sciences/mas-962-special-topics-new-textiles-spring-2010/assignments-and-projects/fabric-pcbs-part-2/assignment-3-pcbutterfly/butterfly_work.jpg)

The PCButterfly in action.

{{< youtube -H-KFf-PNnE >}}

Video of the PCButterfly in action.

Troubleshooting
---------------

We originally used PB5 of the AVR as the sensor pin in our prototype circuit because of location convenience. However, we got very strange behavior of the lights. It turned out that PB5 is also the reset pin, which resets the chip every time it's pulled low, which meant that every time the light turned off, the chip reset. We switched the sensor to PB3, and everything worked fine.

The day before the project was due, we were testing the chip and accidentally shorted power with ground for about 30 seconds before realizing it. Doing that killed the chip, and we were left with a butterfly with 3 LEDs that flickered erratically and wasn't responsive to light. Luckily, we had extra material and made another one. If we were to iterate on the design, we would hide the ground wire so that clipping to VCC cannot possibly touch the ground.

It is relatively easy to dislodge the soldered connections with minor manipulation. It is very useful to have a multi-meter on hand to test individual connections.

| « Previous: [student work sample]({{< baseurl >}}/sections/assignments-and-projects/fabric-pcbs-part-2/fractal-tree-bag) | Next: Return to [Assignment 3 description]({{< baseurl >}}/sections/assignments-and-projects/fabric-pcbs-part-2) »