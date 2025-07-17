# Landmark Research Report: Trends and Relationships in Exoplanet Characteristics and Discoveries

### Introduction

This report presents a foundational analysis of 50 recently discovered exoplanets to explore how **planetary properties relate to host stars and discovery methods.** By examining visualizations and dataset features, we reveal trends in planet radius, mass, equilibrium temperature, and discovery patterns over time. The goal is to understand the astrophysical implications and observational biases shaping our current exoplanet catalog.

### Dataset Overview and Feature Engineering
	•	Size: 50 exoplanets with 8 key features: planet name, discovery method, discovery year, orbital period, radius, mass, equilibrium temperature, and host star spectral type.
	•	Data quality: No missing values; wide ranges in radius (0.7–20.8 Earth radii) and mass (0.5–9,000 Earth masses).
	•	New columns added:
	    •	hostname (star system name),
    	•	planet_count (number of planets in system),
	    •	temp_category (temperature bins: Cool, Medium, Hot).

### Insights from Key Visualizations and Data

1. **Trends in Planet Radius**
	•	Distribution is heavily skewed toward smaller radii with a peak at 1–4 Earth radii.
	•	A bimodal distribution is evident, with peaks near ~2 Earth radii (super-Earths/sub-Neptunes) and ~13 Earth radii (gas giants).
	•	The radius gap (~5–10 Earth radii) suggests differing planet formation/evolution processes or observational biases.
	•	Smaller planets tend to be rocky or Neptune-like; larger planets are likely gas giants.

2. **Temporal Trends in Exoplanet Discoveries**
	•	Discovery counts peaked between 2016 and 2020, with significant dips in 2022 and 2025.
	•	Variations can be attributed to:
	•	Mission lifecycles (e.g., TESS, Kepler),
	•	Pandemic disruptions impacting observations,
	•	Shifts toward detailed characterization of known planets.

3. **Planet Mass vs. Equilibrium Temperature, Colored by Radius**
	•	Most planets cluster at low mass (<100 Earth masses) and moderate temperature (500–1500 K).
	•	Outliers with very high mass (~9000 Earth masses) correspond to large-radius gas giants or brown dwarf candidates.
	•	Larger-radius planets are generally hotter and more massive, consistent with “hot Jupiters” inflated by stellar irradiation.
	•	Radius correlates positively with mass and equilibrium temperature but with considerable scatter.

4. **Planet Mass vs Radius by Discovery Method**
	•	Transit method dominates, detecting primarily smaller (<1000 Earth masses), less massive planets.
	•	Direct Imaging discovers massive, large-radius planets far from host stars.
	•	Radial Velocity is underrepresented but typically detects massive, close-in planets.
	•	The mass-radius relationship shows significant diversity, indicating a range of planetary compositions.

5. **Distribution of Planet Mass**
	•	Mass distribution is strongly right-skewed; most planets have masses below 500 Earth masses.
	•	High-mass planets are rare and primarily detected by imaging methods.

6. **Distribution of Planet Radius**
	•	Reinforces the bimodal distribution with peaks at ~2–3 and 12–15 Earth radii.
	•	Sparse population in the intermediate 5–10 Earth radii range, confirming the “radius gap.”
	•	Very large planets (>15 Earth radii) are rare and correspond to directly imaged exoplanets.

### Synthesis: Relationships and Implications

The analysis reveals several important relationships between exoplanet properties, discovery methods, and host star characteristics. Planet radius displays a bimodal distribution, with clear peaks around 2 Earth radii—corresponding to small rocky or Neptune-like planets—and around 13 Earth radii, representing gas giants. This suggests two dominant classes of exoplanets shaped by their formation and evolutionary processes.

Temporal trends show that exoplanet discovery rates peaked between 2016 and 2020, likely driven by active observation campaigns from missions such as TESS and Kepler. Subsequent declines after 2021 may reflect mission completions, the impact of the COVID-19 pandemic on astronomical observations, and shifts in research focus toward detailed characterization rather than discovery.

The relationship between planet mass, equilibrium temperature, and radius supports the presence of “hot Jupiters”—large, highly irradiated gas giants with inflated atmospheres. Larger-radius planets generally exhibit higher masses and equilibrium temperatures, though the data also show considerable diversity, indicating a wide range of planetary compositions from rocky to gas-dominated worlds.

Discovery methods strongly bias the types of exoplanets detected. Transit surveys primarily find smaller, close-in planets with shorter orbital periods, due to the periodic dips in starlight they cause. Direct imaging is more sensitive to massive, large-radius planets at wider orbital separations. Radial velocity detections, though limited in this dataset, traditionally favor massive planets close to their stars.

Although host star properties were not directly analyzed here, inferred biases suggest that stellar brightness, age, and proximity play significant roles in shaping the observed exoplanet population, as these factors affect detection sensitivity.

### Final Conclusions

	•	The exoplanet population discovered recently is dominated by small, rocky or Neptune-like planets and large, highly irradiated gas giants.
	•	Discovery methods significantly bias the types of planets detected:
    	•	Transit surveys excel at finding smaller, close-in planets with short orbital periods.
    	•	Imaging uncovers massive, large-radius planets at wider orbital separations.
    	•	Radial velocity tends to find massive planets close to stars but is underrepresented here.
	•	Temporal trends reflect both external constraints (missions, global disruptions) and internal shifts in research priorities.
	•	Evidence suggests planet radius and mass are influenced by equilibrium temperature, highlighting the role of stellar irradiation in atmospheric inflation.
	•	Future analyses should integrate orbital period, host star mass/type, and discovery method classification for deeper insight.

### Hypothesis

The observed distribution of exoplanet characteristics, such as radius and mass, is significantly influenced by both intrinsic astrophysical factors (e.g., planet formation processes and stellar irradiation) and observational biases arising from different discovery methods. Specifically, the bimodal radius distribution and correlations between planet mass, radius, and equilibrium temperature reflect a combination of genuine planetary diversity and detection limitations inherent in current survey techniques.

### Next Steps
	•	Conduct multivariate regression and clustering to model planetary characteristics.
	•	Visualize correlations via heatmaps and explore host star-planet interactions.
