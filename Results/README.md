## Correlation Matrix Analysis

This heatmap shows the correlation between key well log parameters and pore pressure (Bower and Eaton).

### High Correlation

- **Eaton_PP and Bower_PP (0.82):** A strong correlation suggests both methods produce consistent pressure estimations.  
- **HP (Hydrostatic Pressure) and Eaton_PP (0.99):** Indicates Eaton’s pore pressure model is highly sensitive to hydrostatic pressure variations.  
- **Sonic and Velocity (-1.00):** A perfect negative correlation, as expected, since velocity increases with compacted formations.  

### Low Correlation

- **Gamma Ray (GR):** Shows minimal correlation with pore pressure (-0.10 to 0.20), indicating limited direct influence on pressure estimations.  

### Significance

- Highlights the most influential parameters for pore pressure prediction, such as hydrostatic pressure, sonic velocity, and density.  
- Negative correlations (e.g., between sonic and pressure) are essential for calibrating predictive models.  
- Helps optimize input variables for advanced machine learning models, reducing redundancy while maximizing predictive power.

