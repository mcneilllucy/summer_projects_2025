# Particle data : globular cluster simulations using NBODY6

We want to use VR to visualise gravitational NBODY simulations of globular clusters (e.g. [Aarseth 2003](https://ui.adsabs.harvard.edu/abs/2003gnbs.book.....A/abstract), [Trenti and Hut 2008](https://arxiv.org/abs/0806.3950)) made with NBODY6.

We take a simulation of a N = 200,000 globular cluster model from [de Vita, Trenti and MacLeod 2019](https://ui.adsabs.harvard.edu/abs/2019MNRAS.485.5752D/abstract). This model, can200k (for 'canonical') is one of a suite of around 20 simulations. The initial setup for can200k used standard assumptions about stellar evolution such as black hole and neutron star birth kicks. It has a metallicity of 0.002, where corresponding stellar wind prescriptions for the black hole progenitor stars consequently gives some specific black hole initial to final mass.

## Project overview

There is a single snapdata.hdf5 file which contains e.g position and velocity vectors of every single star in the simulation. This file is ~100GBs so that analysis beyond this visualization may be slow on commercial laptops.

There are also n_output.dat (e.g. 0_output.dat ... 4_output.dat) files which give a summary of all noteworthy events (such as binary mergers, ejections) per timestep.

### Exercise 1: Formation of black holes in the "mass gap" by hierarchical mergers in dense globular clusters

Summarise the time evolution of the black hole population e.g.

- How many black holes are in the cluster as a function of time? (N vs t)
- What is the mass distribution of the black holes as a function of time?
- Are there any binary black hole mergers? What are the component masses? What is the remnant mass?
- Are there any binary black hole ejections from the globular cluster?
- What is the most massive black hole mass in the simulation (in or out of cluster)?
- Are there any binary neutron star mergers?
- Are there any binary neutron star ejections?

### Exercise 2: Visualizing 3D particle data in 2D

- Plot the black hole population in the x-y plane for several Gyr snap shots
- Plot the neutron star population in the x-y plane for several Gyr snap shots
- Make a movie overlying these two

### Challenge

- Make a 3D movie (i.e. 3D scatter plot) from 0 - 14 Gyr showing the time evolution of the black hole population's position.
- For the black holes, give their markers the physically correct size R ~ m
- For times corresponding to a black hole binary or neutron star binary (i) ejection, or (ii) merger, hold this frame for a few seconds.
- For any frame corresponding to a black hole merger or ejection, plot the velocity vector of the black hole merger remnant / binary in these frames.


# Grid based hydrodynamics solver data : 3D simulations of pre-supernova massive stars with spherical polar geometry using PROMETHEUS (HD) and CoCoNuT-FMT (MHD)

We want to visualise simulations of core-collapse progenitors (e.g. [Müller et al. 2016](https://ui.adsabs.harvard.edu/abs/2016ApJ...833..124M/abstract)) with VR.

One commonly used software for 3D visualization is [VisIt](https://visit-dav.github.io/visit-website/index.html).

## Project overview

In particular, we are interested stellar oscillations in the lead up to core collapse. For example, Figure 2 in [McNeill and Müller 2021](https://ui.adsabs.harvard.edu/abs/2020MNRAS.497.4644M/abstract) shows radial velocities on the left (in the cubed root of km/s), and entropy (in kB/nucleon) on the right. These 2D cross-sections were made in ViSit around 5.5 minutes into the simulation.

This star is a neutron star progenitor during oxygen shell burning. Convection in the low entropy oxygen shell is extremely violent, so that the spherical shell's boundary has a "bubbling" kind of topology. We are interested in the buoyancy waves generated at this boundary, which may propagate in the convectively stable region outside the purple boundary (~4,000 km) until the convective carbon shell ~7,000 km. The set of four up and down drafts may indicate a 4th order stellar oscillation mode.

The following Figure is the absolve value of the radial velocity.

[<img alt="alt_text" width="40px" src="{{ BASE_PATH }}/assets/images/convection-he3.png" />](https://www.google.com/)

Taken in conjunction with the up and down motions, we can see maxima in the radial velocity in the carbon shell. These wave fronts appear to be second order oscillations.

### Exercise 1: Plotting 3D core-collapse progenitor models with VisIt
