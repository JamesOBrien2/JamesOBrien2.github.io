---
layout: post
title: Calculating and visualising Moore O'Ferrall Jencks Plots
date: 2025-11-18 14:13:00
description: This is a post describing the steps required for calculating and visualising 2D potential energy surfaces known as Moore O'Ferrall Jencks Plots.
tags: Tutorial
categories: tutorials
---

# Theory

A Moore O'Ferrall Jencks plot requires the complete scan of two variables, resulting in N^2 scaling. In doing so, a 2D plot can be obtained. An exmaple of where this can be beneficial is in catalysis, where for a bidentate catalyst, you may want to scan the rotational energy barrier of both catalytic arms, to identify the total energetic profile of the system for conversion between cis / trans configurations. (Insert example figure below)

# Calculating the 2D scan

Due to the N^2 scaling of scans over two variables, it is typical and recommended to use either semi-empirical or ML-based methods for these scans. As such, you can anticipate lower than DFT-based energy accuracies, however this will ensure the ability to completely map out the 2D scan.

## Example: Rotational barriers from Cis/Trans orientations of the arms in an organocatalytic system.

```
! xTB ALPB(THF)
%geom
  scan D x x x x = 10, -350, 18 end
  scan D x x x x = 10, -350, 18 end
end
* xyzfile 0 1 inp.xyz
```

# Visualising the 2D scan

lorem Ipsum Lorem Ipsum...
