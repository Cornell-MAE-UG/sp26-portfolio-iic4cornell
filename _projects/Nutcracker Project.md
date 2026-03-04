---
layout: project
title: Nutcracker Problem
description: Nutcracker portfolio
technologies: [MATLAB, python]
image: /assets/images/Nutcracker_part_1.png 
        /assets/images/Nutcracker_part_2.png

---

Problem Statement and Objective:

    Imaging you have a macademia nut that you want to crack open by hand using a simple lever nut cracker. Calculate the necessary dimensions of the nutcracker and come up with a design to make this task feasible


Constraints and Input Parameters:

    Size for Macademia Nuts: 17mm

    Load Needed to Crack a Macademia Nut: 222.18kg

    Max Grip Strength: 550N


Plan:

    1. FBD of nut cracker

    2. FBD of half of the nut cracker

    3. Calculate Fc based on load needed to crack nut

    4. Sum of the moments about point A to find L2


Assumptions:

    1. For simplification, L1, which is the length from the joint to the location of Fc, was set to be the radius of the macademia nut.

    2. The load needed to crack the nut was multiplied by the acceleration due to gravity and rounded to be around 2180N. Fc was then obtained by dividing this by 2 because there are 2 handles.

    3. Force of the handle is equally distributed across the two handles, so the max grip strength can be divided by 2.


Calculations/Thought Process:

    1. Load needed: 222.18kg

        F=(222.18kg)(9.81m/s^2) = 2179.5858N

        F=2180N

        Fc=2180/2 = 1090N

    2. Max grip strenth: 550N

        Fhandle = 550/2 = 275N

    3. Sum of moments about A:

        (8.5mm)(1090N)-(L2)(275N) = 0

        (1090N)(8.5mm) = 275L2
        
        L2 = 33.69mm
    
    Therefore, the Length of the handle should be at least 33.69mm.


Usability:

    Mechanical Advantage = Fc/Fhandle

    Mechanical Advantage = 1090N/275N = 4
    

    The design is usable because of the mechanical advantage, which is greater than 1. Though longer handles could improve the comfort of cracking the macademia nut, 33.60mm as the length of the handle with 550N of max grip is enough to crack the nut, making the design overall usable.



