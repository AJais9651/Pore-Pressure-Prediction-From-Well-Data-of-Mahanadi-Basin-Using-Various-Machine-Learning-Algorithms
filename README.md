 Pore-Pressure-Prediction-From-Well-Data-of-Mahanadi-Basin-Using-Various-Machine-Learning-Algorithms


 Importance of Pore Pressure Prediction
 
•	Pore pressure (PP) represents hydraulic forces in the pore spaces of porous rock formations.

•	Overpressure occurs when PP exceeds recommended levels, posing risks to wellbore stability and drilling safety.

•	Accurate PP forecasting is critical for maintaining drilling safety and ensuring wellbore stability.

Machine Learning in Pore Pressure Prediction

•	Empirical Approaches:

o	Eaton and Bower's methods are employed to estimate vertical stress (𝜎𝑣), PP, and hydrostatic pressure (HP).
o	Inputs include petrophysical logs: density, gamma ray, sonic log, and P-wave velocity.

•	Machine Learning Models:

o	Models used: Random Forest (RF), Extreme Gradient Boosting (XGB), K-Nearest Neighbors (KNN), and Decision Tree (DT).

o	Input combinations: 

1.	Sonic, density, velocity, and gamma logs.
2.	Sonic, density, velocity, gamma logs + hydrostatic pressure.
3.	Sonic, density, velocity, gamma logs + previous depth pore pressure.

o	ML models are trained separately using Eaton's and Bower's PP estimations as targets.

o	Datasets from wells NGHP-01-8A and NGHP-01-19B in the Mahanadi Basin are analyzed.

Study Area: Mahanadi Basin

•	Gas Hydrates:

o	Icy substances formed when gas is trapped within water's molecular structure under high pressure and low temperature.

o	Found in two forms: filling pores/replacing grains or filling fractures.

o	Significant sand input and organic-rich sediments make the basin favorable for gas hydrates.

•	Velocity Characteristics:

o	Increased velocity correlates with higher hydrate content in sediments.

o	Below the gas hydrate stability zone (GHSZ), velocity decreases due to free gas compressibility.
Bottom-Simulating Reflector (BSR)

•	Significance: 

o	BSR helps identify gas hydrates through seismic reflections.

o	Indicates polarity difference due to contrasting properties of gas hydrate and free gas layers.

o	Often intersects structural and stratigraphic reflections, aiding geological identification.

o	Absence of BSR does not confirm the absence of gas hydrates.
    Petrophysical Log Observations

•	Within GHSZ: 

o	Higher P-wave velocity, resistivity, and density.

o	Gamma log values (65–160 API) suggest clay or silt presence.

•	Below GHSZ: 

o	P-wave velocity peaks just below GHSZ and then drops abruptly.
Well Details and BSR Depths

•	Well NGHP-01-19B: 

o	Seafloor: 1433 m.

o	BSR: 208 m below seafloor (mbsf).

•	Well NGHP-01-8A: 

o	Seafloor: 1701 m.

o	BSR: 257 mbsf.

•	BSR depths are marked with dashed yellow lines for clarity.

