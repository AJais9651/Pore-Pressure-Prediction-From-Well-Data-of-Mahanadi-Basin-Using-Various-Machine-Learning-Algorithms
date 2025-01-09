# Importance of Pore Pressure Prediction

Pore pressure (PP) represents the hydraulic forces within the pore spaces of porous rock formations. Overpressure occurs when PP exceeds recommended levels, posing significant risks to wellbore stability and drilling safety. Accurate PP forecasting is critical for maintaining drilling safety and ensuring wellbore stability.

---

## Machine Learning in Pore Pressure Prediction

### Empirical Approaches
- **Eaton and Bower's Methods**: These are commonly employed to estimate vertical stress (σ_v), pore pressure (PP), and hydrostatic pressure (HP).
- **Inputs**: Petrophysical logs, including density, gamma ray, sonic log, and P-wave velocity.

### Machine Learning Models
- **Models Used**:
  - Random Forest (RF)
  - Extreme Gradient Boosting (XGB)
  - K-Nearest Neighbors (KNN)
  - Decision Tree (DT)
- **Input Combinations**:
  1. Sonic, density, velocity, and gamma logs.
  2. Sonic, density, velocity, gamma logs + hydrostatic pressure.
  3. Sonic, density, velocity, gamma logs + previous depth pore pressure.
- **Model Training**:
  - Machine learning models are trained separately using Eaton's and Bower's PP estimations as targets.
- **Dataset**:
  - Data from wells NGHP-01-8A and NGHP-01-19B in the Mahanadi Basin were analyzed.

---

## Study Area: Mahanadi Basin

### Gas Hydrates
- **Definition**: Icy substances formed when gas is trapped within water's molecular structure under high pressure and low temperature.
- **Occurrence**: Found in two forms:
  1. Filling pores/replacing grains.
  2. Filling fractures.
- **Favorable Conditions**: Significant sand input and organic-rich sediments make the Mahanadi Basin ideal for gas hydrates.

### Velocity Characteristics
- Increased velocity correlates with higher hydrate content in sediments.
- Below the gas hydrate stability zone (GHSZ), velocity decreases due to free gas compressibility.

### Bottom-Simulating Reflector (BSR) Significance
- **Role**: Helps identify gas hydrates through seismic reflections.
- **Polarity Difference**: Indicates contrasting properties of gas hydrate and free gas layers.
- **Geological Identification**: Often intersects structural and stratigraphic reflections.
- **Absence of BSR**: Does not confirm the absence of gas hydrates.

---

## Petrophysical Log Observations

### Within GHSZ
- Higher P-wave velocity, resistivity, and density.
- Gamma log values (65–160 API) suggest clay or silt presence.

### Below GHSZ
- P-wave velocity peaks just below GHSZ and then drops abruptly.
- **Observations**:
  - Pore pressure increases with depth to maintain hydrostatic balance.
  - A small rise in pore pressure around the BSR suggests the presence of free gas below the gas hydrate zone.

---

## Well Details and BSR Depths

- **Well NGHP-01-19B**:
  - Seafloor: 1433 m.
  - BSR: 208 m below seafloor (mbsf).
- **Well NGHP-01-8A**:
  - Seafloor: 1701 m.
  - BSR: 257 mbsf.

---

## Effective Stress Rule (Terzaghi and Biot)

### Key Definitions
- **Effective Stress (σ_e)**: Stress that directly impacts rock grains and controls compaction and strength.
- **Overburden Stress (σ_v)**: Total stress exerted by the weight of overlying sediments, including the rock and water above the measurement point.
- **Pore Pressure (PP)**: Pressure of fluids (like water or gas) within the pores of the sediment or rock.

### Equation
\[
PP = \frac{(\sigma_v - \sigma_e)}{\alpha}
\]
Where:
- \(\alpha\): Biot's effective stress coefficient, accounting for how pore pressure supports the overburden load.

---

## Eaton’s Method for Pore Pressure Prediction

### Vertical Stress (\(\sigma_v\))
- **Dependence**: Vertical stress depends on the weight of sediments and water above the measurement point.
- **Formula**:
\[
\sigma_v = \rho_s h g + \int_k^z \rho(z) g \, dz
\]
Where:
- \(g\): Acceleration due to gravity (9.852 m/s²).
- \(\rho(z)\): Density of sediments with depth.
- \(h\): Seabed depth.
- \(z\): Depth below the ocean floor.

### Normal Compaction Trend
As sediments get buried, they compact under increasing overburden stress, reducing porosity and altering properties like sonic travel time.

### Eaton’s Sonic Method
- **Formula**:
\[
PP_{\text{eaton}} = \sigma_v - (\sigma_v - P_h) \cdot \left(\frac{DT_n}{DT}\right)^3
\]
Where:
- \(P_h\): Hydrostatic pressure (pressure from seawater above).
- \(DT_n\): Sonic travel time in a low-permeability, normally compacted zone.
- \(DT\): Observed sonic travel time in the target zone.

---

## Bower’s Method

### Key Concepts
1. **Effective Stress Equation**:
\[
\sigma_e = \sigma_v - PP
\]
Where:
- \(\sigma_v\): Overburden stress.
- \(PP\): Pore pressure.

2. **Bower’s Velocity-Effective Stress Model**:
\[
\sigma_v - PP = \left(\frac{V - V_o}{a}\right)^{1/b}
\]
Where:
- \(V\): Observed velocity.
- \(V_o\): Velocity at the seafloor.
- \(a\) and \(b\): Fitting parameters (calculated from data).

3. **Logarithmic Form**:
- By taking the logarithm of the equation, it becomes linear: \(Y = bX + C\), allowing for a linear fit to find \(a\) and \(b\).

4. **Results**:
- Figures 1 to 16 show the estimated pore pressures for Wells NGHP-01-08A and NGHP-01-19B using both Bower’s and Eaton’s methods.

---

## Lines Representing Different Parameters

- **Blue Line (Pore Pressure - Bower)**: Pore pressure calculated using Bower's method.
- **Red Line (Vertical Stress)**: Represents overburden stress (\(\sigma_v\)), including the weight of overlying sediments.
- **Green Dashed Line (Hydrostatic Pressure)**: Baseline pressure due to seawater above.
- **Magenta Line (Pore Pressure - Eaton)**: Pore pressure calculated using Eaton's method.
- **Yellow Dashed Line (BSR Depth)**: Marks the Bottom-Simulating Reflector (BSR) depth (~208 mbsf).

### Hydrostatic Pressure (Green Dashed Line)
- Represents the baseline pressure exerted by seawater. Any deviation above it indicates overpressure.

### Pore Pressure (Blue and Magenta Lines)
- Pore pressure values derived using Bower's and Eaton's methods generally align but show variations depending on the method and depth. Deviations from hydrostatic pressure signify potential overpressure zones.

### Vertical Stress (Red Line)
- Represents the total overburden stress. As expected, pore pressure remains below this line since it only partially supports the overburden.

### BSR Depth (Yellow Dashed Line)
- Indicates the presence of the gas hydrate stability zone (GHSZ) above the BSR and a free gas zone below it.

---

## Significance of the Figure

1. **Overpressure Detection**: The difference between the pore pressure (blue/magenta) and hydrostatic pressure (green dashed line) identifies overpressure zones.
2. **Hydrate Zone Assessment**: The BSR marks a critical boundary where gas hydrates are stable above, and free gas is present below.
3. **Comparison of Methods**: The alignment and divergence of Bower's and Eaton's methods provide insight into the reliability and accuracy of the approaches.



