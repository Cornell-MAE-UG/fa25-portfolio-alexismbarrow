---
layout: project
title: MAE 3270: Mechanics of Materials
description: FEA + CAD modeling Final Project
technologies: [Autodesk Fusion, ANSYS]
image: ![CAD img]({{ "assets/images/mae3270-cad.png" | relative_url }}){: class="profile-image"}
---



For the class MAE 3270, Mechanics of Materials, we were tasked to solve an engineering problem: building a torque wrench that could undergo a certain set of conditions, which were as follows:

- Withstand a torque of 600 in-lbf for 10^6 cycles. 
- At least 1 mV/V output at the rated torque.
- A safety factor of at least 4 for yield or brittle failure.
- A safety facor of at least 2 for crack growth from an assumed crack depth of 0.04 in.
- A fatigue stress safety factor of at least 1.5
- Be made from a steel, aluminum, or titanum alloy.
- Have a driver with dimensions 0.375in x 0.375in x 0.5in

From this, we were to firstly use hand calculations to find a suitable design. We were to, after this, build our model in CAD, and use FEA to validate our results.

Firstly, an image of the CAD with all key dimensions:

![CAD img]({{ "assets/images/mae3270-cad.png" | relative_url }}){: class="profile-image" "width: 100%"}


Image indicating how loads and boundary conditions were applied to the FEM model:

![question 3]({{ "assets/images/q3.png" | relative_url }}){: class="profile-image"}

Normal strain contours from FEM:
![question 4]({{ "assets/images/q4.png" | relative_url }}){: class="profile-image"}
![question 4.2]({{ "assets/images/q4-2.png" | relative_url }}){: class="profile-image"}


Contour plot of maximum principal stress from FEM:

![question 5]({{ "assets/images/q5-1.png" | relative_url }}){: class="profile-image"}
![question 5-2]({{ "assets/images/q5-2.png" | relative_url }}){: class="profile-image"}

Maximum normal stress:

![question 6-1]({{ "assets/images/q6-1.png" | relative_url }}){: class="profile-image"}
![question 6-2]({{ "assets/images/q6-2.png" | relative_url }}){: class="profile-image"}


The load point deflection, pictured below, is 0.2267 for the faces of the driver. They are defined as fixed supports due to the nature of the purpose of the torque wrench. Assuming it is not being twisted beyond its capacity (which would incur a frictionsl contact support), none of the faces of the driver will move. This principle causes a case in which the load is not distributed down into the driver, but rather concentrated in the end of the handle, where the load is applied. 

Load point deflection: 
![question 7]({{ "assets/images/q7.png" | relative_url }}){: class="profile-image"}
The load point deflection, pictured below, is 0.2267 for the faces of the driver. They are defined as fixed supports due to the nature of the purpose of the torque wrench. Assuming it is not being twisted beyond its capacity (which would incur a frictionsl contact support), none of the faces of the driver will move. This principle causes a case in which the load is not distributed down into the driver, but rather concentrated in the end of the handle, where the load is applied. 

Strains at the strain gauge locations:
![question 7-2]({{ "assets/images/q7-2.png" | relative_url }}){: class="profile-image"}
The strain gauges are located approximately 1 inch from the center of the driver along the x-axis. The maximum strain measured is 1.9342e-003, and it occurs partway up the driver.

Torque wrench sensitivity in mV/V using strains from the FEM analysis:

![question 7-3]({{ "assets/images/q7-3.png" | relative_url }}){: class="profile-image"}

![question 7analysis]({{ "assets/images/q7analysis.png" | relative_url }}){: class="profile-image"}

Strain Gauge Selected: SGD-2/350-LY11 Linear Strain Gauge from DwyerOmega
![question strain gauge]({{ "assets/images/StrainGaugePic" | relative_url }}){: class="profile-image"}
Dimensions: 7.6mm (0.3in) x 5.8mm (0.23in)
