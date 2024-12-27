**Importance of Pore Pressure Prediction
•	Pore pressure (PP) represents hydraulic forces in the pore spaces of porous rock formations.
•	Overpressure occurs when PP exceeds recommended levels, posing risks to wellbore stability and drilling safety. Accurate PP forecasting is critical for maintaining drilling safety and ensuring wellbore stability.
**Machine Learning in Pore Pressure Prediction
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
o	Significant sand input and organic-rich sediments make the basin favourable for gas hydrates.
•	Velocity Characteristics:
o	Increased velocity correlates with higher hydrate content in sediments.
o	Below the gas hydrate stability zone (GHSZ), velocity decreases due to free gas compressibility.

Bottom-Simulating Reflector (BSR) Significance: 
o	BSR helps identify gas hydrates through seismic reflections.
o	Indicates polarity difference due to contrasting properties of gas hydrate and free gas layers.
o	Often intersects structural and stratigraphic reflections, aiding geological identification.
o	Absence of BSR does not confirm the absence of gas hydrates.

**Petrophysical Log Observations
•	Within GHSZ: 
o	Higher P-wave velocity, resistivity, and density.
o	Gamma log values (65–160 API) suggest clay or silt presence.
•	Below GHSZ: 
o	P-wave velocity peaks just below GHSZ and then drops abruptly.
o	Observations: 
	Pore pressure increases with depth to maintain hydrostatic balance.
	Around the BSR, there’s a small rise in pore pressure, suggesting the presence of free gas below the gas hydrate zone.

Well Details and BSR Depths
•	Well NGHP-01-19B: 
o	Seafloor: 1433 m.
o	BSR: 208 m below seafloor (mbsf).
![image](https://github.com/user-attachments/assets/113df9c1-57a6-44d5-9f13-764a3ce0346b)

•	Well NGHP-01-8A: 
o	Seafloor: 1701 m.
o	BSR: 257 mbsf.
![image](https://github.com/user-attachments/assets/95020681-a838-43b5-ad08-ee273bef840f)


**Effective Stress Rule (Terzaghi and Biot):
•	Effective Stress (σe): The stress that directly impacts the rock grains and controls compaction and strength.
•	Overburden Stress (σv): The total stress exerted by the weight of overlying sediments, including the rock and water above the measurement point.
•	Pore Pressure (PP): The pressure of fluids (like water or gas) within the pores of the sediment or rock.

Equation:     PP=(σv−σe)/α
α: Biot's effective stress coefficient, which accounts for how pore pressure supports the overburden load.
Eaton’s Method for Pore Pressure Prediction:
Vertical Stress (σv):
o	Vertical stress depends on the weight of sediments and water above the measurement point.
o	It's calculated using:
                             Where: 
	g = acceleration due to gravity (9.852 m/s²),
	ρ(z) = density of sediments with depth,
	h = seabed depth,
	z = depth below the ocean floor.
Normal Compaction Trend:
As sediments get buried, they compact under increasing overburden stress, which reduces porosity and changes properties like sonic travel time.
![image](https://github.com/user-attachments/assets/3dead9f1-c215-42c9-bebe-28508fb17795)


![image](https://github.com/user-attachments/assets/81eee21e-86c2-4ebe-bf40-e65e06d4e917)



Eaton’s Sonic Method:Uses sonic compressional travel time to estimate pore pressure:
 
Ph = hydrostatic pressure (pressure from seawater above),
DTn = sonic travel time in a low-permeability, normally compacted zone,
DT = observed sonic travel time in the target zone.

Bower's Method:
This is an advanced approach to predicting pore pressure based on effective stress and wave velocities.
Key Concepts:
1.	Effective Stress Equation:
o	Effective stress is calculated as: σe=Sv−PP
Where: 
	Sv: Overburden stress,
	PP: Pore pressure.

2.	Bower's Velocity-Effective Stress Model:
o	This method relates effective stress to seismic wave velocity.
o	The relationship is expressed as: 
Where: 
	V: Observed velocity,
	Vo: Velocity at the seafloor,
	a and b: Fitting parameters (calculated from data).
3.	Logarithmic Form:
o	By taking the logarithm of the equation: 
o	The equation becomes linear (Y= bX + C) and can be plotted as: 
This allows for a linear fit to find a and b, as shown in Figures.

4.	Results:
o	Figures 1 to 16 show the estimated pore pressures for Wells NGHP-01-08A and NGHP-01-19B using both Bower’s and Eaton’s methods.
![image](https://github.com/user-attachments/assets/539023cc-061a-4836-83cd-c42c286a9517)
![image](https://github.com/user-attachments/assets/fe62e0b2-b783-49d4-b362-0407b304aef1)
![image](https://github.com/user-attachments/assets/baf609f4-acf0-490c-a12e-8dafc8fca6ab)
![image](https://github.com/user-attachments/assets/7839a8b7-5985-4715-a568-1652fcadac4a)


6.	Conclusions:
 ![image](https://github.com/user-attachments/assets/2317db7e-ff61-4f60-88c9-85b502a1512c)

1.	Prediction accuracy improves with the number of input logs used for training in both wells.
2.	Models perform well with sonic, density, velocity, and gamma-ray logs, but accuracy increases further when Eaton's pore pressure and hydrostatic pressure are included in the training.
3.	Random Forest outperforms K-Nearest Neighbors, Decision Tree, and Extreme Gradient Boosting models.
4.	Using Eaton’s method with sonic, density, velocity, gamma, and hydrostatic pressure as inputs yields the best accuracy for Well 8 with the Random Forest model (Fig. 17).
5.	This study provides new insights into geomechanical processes in gas hydrate zones.


