---
title: "Neutron Density Visualization"
excerpt: "Visualizing neutron flux in nuclear reactors for optimizing fuel rod geometry<br/><img src='/images/553_viz.png'>"
collection: portfolio
---

![alt_text](/images/553_viz.png)

Understanding the distribution of neutrons inside a reactor core is essential for nuclear reactor design. The interaction of these neutrons determine optimal fuel rod placement and geometry. Using [MCNP 6.2](https://rsicc.ornl.gov/codes/ccc/ccc8/ccc-850.html), Monte Carlo simulation package, we generate the position of neutrons given various fuel rod designs.

Using these simulations, we take the point cloud data from MCNP6.2 and generate a scalar field, using [Delaunay triangulation](https://en.wikipedia.org/wiki/Delaunay_triangulation) to create a geometry. From here, we use OpenGL to visualize this data. Our visualization technique uses RGB color mapping and height mapping to demonstrate neutron density at various level sets.

[You can see the source code here.](https://github.com/Aidan-B1409/neutron_flux_visualization)


