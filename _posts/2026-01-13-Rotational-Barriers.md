---
layout: post
title: Calculating Rotational Barriers (1D Dihedral Scans)
date: 2026-01-13 11:58:00
description: This is a post describing the steps involved in calculating rotational barriers via dihedral bond rotations.
tags: Tutorial
categories: tutorials
---

# Important

Although this tutorial is applied to complex systems, This tutorial details the simplified 1D PES scan of a dihedral angle to obtain rotational barriers. For more complex systems involving multiple dihedral angles, please refer to the Moore O'Ferrall Jencks Plot tutorial.

# Finding the correct dihedral angle

The first step in calculating rotational barriers is to identify the dihedral angle of interest. This can typically be done using molecular visualization software to inspect the 3D structure of the molecule and select the four atoms that define the dihedral angle. It is important to ensure that the selected atoms accurately represent the rotational axis you wish to study. For example, to identify the rotational barrier for a catalyst arm to convert from monodentate to bidentate binding mode, you would select the atoms involved in the bond rotation that facilitates this change, as shown below:

![Dihedral Angle Example]{{(/assets/img/blogs/dihedral_angle_example.png | relative_url)}}{: style="width:100%; height:auto;"}

# Setup

Once the atoms involved in the dihedral angle have been identified, the next step is to set up a dihedral scan. This involves defining a series of dihedral angles to sample, typically ranging from 0° to 360° in increments (e.g., every 1-10°). The choice of increment size can affect the resolution of the resulting energy profile; smaller increments provide more detail but require more computational resources.

As such, it is recommended to start with small increments (e.g., 1°) with a method that has a low computational cost (xTB). This can be further refined using energies from DFT calculations at the optimized geometries from the initial scan.

# Execution

To perform the dihedral scan using ORCA 6.1, you will need to create an input file that specifies the dihedral scan parameters. Below is an example of how to set up the input file for a dihedral scan:

```plaintext
! XTB ALPB(Water) Opt
%geom
    Scan D 1 2 3 4  = starting_angle, end_angle, number_of_steps end# Replace 1,2,3,4 with the atom indices of the dihedral
end
* xyzfile 0 1 inp.xyz
```

# Interpretation

The resulting `.out` file will contain the electronic energy at each step as shown for an example below:

```
The Calculated Surface using the 'Actual Energy'
 294.00000000 -2480.71412416
 272.94117647 -2480.71435565
 251.88235294 -2480.71443016
 230.82352941 -2480.71226184
 209.76470588 -2480.70414586
 188.70588235 -2480.68771514
 167.64705882 -2480.66203235
 146.58823529 -2480.70618012
 125.52941176 -2480.71301909
 104.47058824 -2480.71448324
  83.41176471 -2480.71452271
  62.35294118 -2480.71382932
  41.29411765 -2480.70877788
  20.23529412 -2480.69684666
  -0.82352941 -2480.67743996
 -21.88235294 -2480.65077805
 -42.94117647 -2480.70932893
 -64.00000000 -2480.71402890
```

Depending on your input file you may also obtain the "Total energy" at each step in the following format:

```
The Calculated Surface using the SCF energy
 294.00000000 -2480.63895087
 272.94117647 -2480.63916453
 251.88235294 -2480.63943315
 230.82352941 -2480.63737013
 209.76470588 -2480.62930300
 188.70588235 -2480.61299020
 167.64705882 -2480.58753095
 146.58823529 -2480.63140782
 125.52941176 -2480.63824869
 104.47058824 -2480.63978587
  83.41176471 -2480.63983061
  62.35294118 -2480.63899664
  41.29411765 -2480.63386712
  20.23529412 -2480.62199031
  -0.82352941 -2480.60278619
 -21.88235294 -2480.57642920
 -42.94117647 -2480.63427118
 -64.00000000 -2480.63892007
```

With these results you are able to plot a typical 2D plot easily using python packages such as `matplotlib` or `plotly`! Although this is not required to denote the maximum energy value which is representative of your rotational barrier!
