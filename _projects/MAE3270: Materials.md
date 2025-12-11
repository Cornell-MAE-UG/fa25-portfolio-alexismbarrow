---
layout: project
title: MAE 3270: Mechanics of Materials
description: FEA + CAD modeling Final Project
technologies: [Autodesk Fusion, ANSYS]
image: /assets/images/mae3270-cad.png
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
<img src="https://alexisbarrow.github.io/fa25-portfolio-alexismbarrow/assets/images/mae3270-cad.png" alt="CAD image" width="600">



Image indicating how loads and boundary conditions were applied to the FEM model:
<img src="https://alexisbarrow.github.io/fa25-portfolio-alexisbarrow/assets/images/q3.png" alt="q3">
E
Normal strain contours from FEM:
<img src="https://alexisbarrow.github.io/fa25-portfolio-alexisbarrow/assets/images/q4.png" alt="q4">
<img src="https://alexisbarrow.github.io/fa25-portfolio-alexisbarrow/assets/images/q4-2.png" alt="q4-2">

Contour plot of maximum principal stress from FEM:
<img src="https://alexisbarrow.github.io/fa25-portfolio-alexisbarrow/assets/images/q5-1.png" alt="q5-1">
<img src="https://alexisbarrow.github.io/fa25-portfolio-alexisbarrow/assets/images/q5-2.png" alt="q5-2">

Maximum normal stress:
<img src="https://alexisbarrow.github.io/fa25-portfolio-alexisbarrow/assets/images/q6-1.png" alt="q6-1">
<img src="https://alexisbarrow.github.io/fa25-portfolio-alexisbarrow/assets/images/q6-2.png" alt="q6-2">
The load point deflection, pictured below, is 0.2267 for the faces of the driver. They are defined as fixed supports due to the nature of the purpose of the torque wrench. Assuming it is not being twisted beyond its capacity (which would incur a frictionsl contact support), none of the faces of the driver will move. This principle causes a case in which the load is not distributed down into the driver, but rather concentrated in the end of the handle, where the load is applied. 

Load point deflection: 
<img src="./assets/images/q7.png">
The load point deflection, pictured below, is 0.2267 for the faces of the driver. They are defined as fixed supports due to the nature of the purpose of the torque wrench. Assuming it is not being twisted beyond its capacity (which would incur a frictionsl contact support), none of the faces of the driver will move. This principle causes a case in which the load is not distributed down into the driver, but rather concentrated in the end of the handle, where the load is applied. 

Strains at the strain gauge locations:
<img src="https://alexisbarrow.github.io/fa25-portfolio-alexisbarrow/assets/images/q6-4.png" alt="q6-4">
The strain gauges are located approximately 1 inch from the center of the driver along the x-axis. The maximum strain measured is 1.9342e-003, and it occurs partway up the driver.

Torque wrench sensitivity in mV/V using strains from the FEM analysis:
<img src="https://alexisbarrow.github.io/fa25-portfolio-alexisbarrow/assets/images/q7.png" alt="q7">
<img src="./assets/images/q7analysis.png">

Strain Gauge Selected: SGD-2/350-LY11 Linear Strain Gauge from DwyerOmega
<img src="./assets/images/StrainGaugePic.png">
Dimensions: 7.6mm (0.3in) x 5.8mm (0.23in)
