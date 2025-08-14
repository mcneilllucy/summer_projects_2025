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


## Example scripts for data analysis

- [ ] ipython notebook
- [ ] .py script

- Results
  - [ ] .csv files for important events e.g. black hole ejections, exchanges


# Grid data : 3D simulations of pre-supernova massive stars with spherical polar geometry using PROMETHEUS (HD) and CoCoNuT-FMT (MHD)

To be added later.
