Stage 1 – Setup & Theoretical Foundation

1.	I will install and verify my Python environment using Anaconda or a dedicated virtual environment, along with JupyterLab for code execution, visualisation, and documentation.

2.	I will install essential scientific and astrodynamics libraries — poliastro, astropy, numpy, matplotlib, and pandas — for orbital computation and plotting.

3.	I will review the theoretical foundations of Mars transfer dynamics, including Kepler’s laws, two-body propagation, Hohmann transfers, synodic periods, and Lambert’s problem.

4.	I will set up access to NASA’s JPL Horizons database through the astroquery.jplhorizons interface or manually export ephemerides for Earth and Mars for defined launch windows.

5.	I will retrieve and inspect the heliocentric positions and velocities of Earth and Mars over a multi-year range to establish the foundation for transfer analysis.

6.	I will plot the heliocentric orbits of Earth and Mars over a 2–3-year window using poliastro.plotting or Matplotlib to visualise orbital geometry and phasing opportunities.

7.	I will define a consistent project folder structure — /data, /scripts, /figures, /results, and /notebooks — to ensure clarity, traceability, and reproducibility.

8.	I will document the data retrieval process, specifying metadata, coordinate reference frames (ICRF, ecliptic), and time systems (JD, MJD, UTC) used in imported datasets.

9.	I will develop a Python script to compute classical orbital elements (a, e, i, Ω, ω, ν) for Earth and Mars directly from JPL data to verify correctness.

10.	I will review key Mars transfer and arrival missions (e.g., MAVEN, Mars Reconnaissance Orbiter, ExoMars) to understand typical ΔV budgets, transfer times, and injection energies.

Stage 2 – Baseline Modelling & Direct Transfers

11.	I will implement a Hohmann transfer approximation between Earth and Mars to establish a baseline reference for energy-optimal transfer.

12.	I will visualise the Hohmann transfer ellipse and the relative orbital positions of Earth and Mars at departure and arrival using Matplotlib and poliastro.

13.	I will develop a Lambert solver function using poliastro.iod.lambert to model realistic transfer trajectories for varying launch and arrival epochs.

14.	I will compute ΔV and time-of-flight (ToF) for a range of candidate launch windows across multiple synodic periods (e.g., 2026–2030).

15.	I will generate a ΔV vs ToF trade plot to identify low-energy transfer opportunities and highlight optimal windows.

16.	I will store all computed trajectories in a structured Pandas DataFrame, including departure epoch, arrival epoch, ΔV values, and orbital parameters.

17.	I will export key trajectory solutions as mission profiles (JSON/CSV) summarizing ΔV breakdowns, C3 energy, and arrival velocity.

18.	I will perform sensitivity analyses by perturbing launch dates (±5–10 days) to quantify timing sensitivity on ΔV requirements.

19.	I will annotate orbit and transfer plots with mission metadata — including launch/arrival epochs, ToF, and ΔV magnitudes — for clear communication.

20.	I will prepare Markdown-based technical notes detailing modelling assumptions, data sources, reference frames, and units (AU, km/s, days).

Stage 3 – Gravity-Assist & Advanced Propagation

21.	I will investigate potential gravity-assist trajectories (e.g., Earth–Venus–Mars) by analysing synodic alignments and planetary geometry.

22.	I will construct a patched-conic, multi-leg trajectory using poliastro to simulate an Earth–Venus–Mars assist profile.

23.	I will numerically propagate both trajectory legs and calculate total ΔV and ToF for comparison against the direct Earth–Mars case.

24.	I will plot both direct and assisted trajectories in 3D to illustrate energy and time advantages.

25.	I will compare chemical vs electric propulsion by assessing mission feasibility given ΔV and available Isp values.

26.	I will include spacecraft mass fraction and payload trade-off analyses using standard rocket equation relations.

27.	I will tabulate trade-offs across propulsion modes, including ΔV, ToF, propellant fraction, and overall mission complexity.

28.	I will run a Monte Carlo–style parameter sweep, varying launch date and eccentricity, to visualise feasible launch windows and mission envelopes.

29.	I will create publication-quality visualisations such as C3 vs Launch Date and Arrival V∞ vs ToF to include in the final report.

30.	I will compile the final technical report, integrating all results, visualisations, methodology, and references — ensuring that each figure, dataset, and source is properly cited.

