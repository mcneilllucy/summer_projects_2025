# Stellar evolution modelling

In this project, we will simulate several models for helium composition white dwarfs with various surface temperatures (around between 4000 K - 30,000 K) using [MESA](https://docs.mesastar.org/en/latest/)

The goal is to plot each model's mass (x-axis) vs its radius (y-axis) plots like [Panei et al. 2000](https://adsabs.harvard.edu/full/2000A%26A...353..970P)'s Figure 3.

We would like to extend this to a 3rd dimension in a z-axis for the *central entropy*.

# White dwarf binaries

99% of stars become white dwarfs. In addition, most of them are in binaries (or multiple systems e.g. triples).

"Short period" white dwarf binaries (orbital periods between a few minutes - 1 hour) usually have one or both components with a Helium composition. As they orbit, these binaries gradually get closer to each other due to energy loss from the emission of gravitational waves. Eventually, they are close enough so that the larger star can no longer contain its material given the gravitational potential of its companion. There (called "Roche lobe overflow" or "Roche contact")

[McNeill and Hirai 2025](https://ui.adsabs.harvard.edu/abs/2025arXiv250721821M/abstract) recently found that observations of short period white dwarf binaries in the Milky Way suggest that helium white dwarfs are typically very hot, and therefore only partially degenerate at the moment they start transferring mass. Mass transfer is classed as dynnamically "stable" or "unstable", depending on whether the merge or not (unstable mass transfer). Mass  transferring white dwarf binaries therefore lead to a variety of astrophysical exotica such as faint type Ia supernova, hot subdwarf stars, AM CVn binaries. So it is important that we study the thermal (temperature, entropy etc.) structure of hot Helium white dwarf binaries.


## Exercises

While we don't have simulations of the helium white dwarfs yet, let's practise some data analysis of stellar evolution models made by MESA.

Let's take a MESA model of a massive star during its most advanced burning phases of oxygen and silicon shell burning. [Aguilera-Dena et al. 2019](https://ui.adsabs.harvard.edu/abs/2018ApJ...858..115A/abstract)

20mso_model.dat is the raw data file.

1. As a function of radius (in km), plot
  - the density (in g / cm^3)
  - The entropy (in units of k_B / nucleon)

Suggestion for getting started:
  - convert 20mso_model.dat to a .csv.
  - manipulate with the "pandas" python library.

2. As a function of enclosed mass (in solar masses), plot
  - the density (in g / cm^3)
  - The entropy (in units of k_B / nucleon)

3. What is the mean density of the whole star?

4. What is the mean density of the region out to a mass coordinate of 1.2 solar masses?
