# Martian-Core-Analysis

## Module 6 - Seismic Data Classification and Shadow Zone Prediction
- *Objective*: This module focuses on extracting key features from seismic waveforms and using them for shadow zone classification on Mars. The classification helps in identifying whether a station falls within a shadow zone, where seismic waves are absent due to the Earth's or Mars' core.
  
- *Key Steps*:
  - *Part 1*: Extract features such as amplitude, frequency, and phase shift from seismic waveform data using signal processing techniques.
  - *Part 2*: Generate a synthetic dataset containing all features relevant for classifying shadow zones, such as source coordinates, depth of the source, P-wave travel time, RMS amplitude, and instantaneous frequency.
  - Label the shadow zones based on astronomical parameters derived from the seismic features.
  - Perform Exploratory Data Analysis (EDA) and preprocessing to clean and normalize the data, ensuring no null values and that all features are numerical.
  - Use Random Forest Classifier to train a model on the dataset with hyperparameter tuning via Randomized Search CV.
  - Predict the station's location (shadow zone or non-shadow zone) based on user inputs such as source coordinates and travel time of seismic waves.

## Module 7 - Regression and Feature Importance Analysis
- *Objective*: This module aims to predict P-wave and S-wave velocities by analyzing the seismic data. It also includes feature importance analysis to identify key factors affecting the predictions and model performance evaluation.

- *Key Steps*:
  - *Feature Importance*: Perform feature importance analysis using a Random Forest model to understand which seismic features are most impactful for predicting wave velocities.
  - *Physics-based Calculation*: Calculate P-wave and S-wave velocities using bulk modulus, shear modulus, and density based on well-known physical formulas.
  - *Outlier Detection*: Identify and handle outliers in the dataset using statistical methods to ensure robust model performance.
  - *Regression Models*: Train several regression models such as Ridge, Lasso, Elastic Net, SVR, and Gradient Boosting Regressor to predict the wave velocities.
  - *Hyperparameter Tuning*: Use Randomized Search CV to fine-tune hyperparameters for better model performance in Ridge, Lasso, Elastic Net, SVR, and Gradient Boosting Regressor models.
  - *Model Evaluation*: Evaluate each model's performance using common metrics like Mean Squared Error (MSE), Mean Absolute Error (MAE), Accuracy, and Mean Absolute Percentage Error (MAPE).

## Module 8 - Seismic Wave Analysis and Interpretation
- *Objective*: This module is focused on interpreting seismic wave data to detect anomalies or geological features that could indicate underlying structures on Mars.

- *Key Steps*:
  - *Vp/Vs Ratio Analysis*: Interpret the Vp/Vs ratio, which can indicate fluid-filled zones, fractured rocks, or other geological formations. Higher or lower-than-expected ratios can help identify regions with fluid pockets, fractured rocks, or ice inclusions.
  - *Poisson's Ratio Analysis*: Analyze the Poisson’s ratio, which can be used to identify the presence of fluids, porous rocks, or gas pockets. Abrupt shifts in Poisson's ratio could indicate stratigraphic changes or faulted regions.
  - *Attenuation Patterns*: Study seismic attenuation, which reveals energy loss in different regions. High attenuation suggests loose sediments or gas-rich layers, while low attenuation indicates compact, dense formations such as basaltic bedrock.
  - Use sudden changes in seismic data (such as drops in Vp and Vs) to detect weak zones, unconsolidated sediments, or faulted regions.

## Module 9 - GAN-based Data Generation and Prediction
- *Objective*: This module employs a Generative Adversarial Network (GAN) to generate synthetic Martian seismic data for P-wave and S-wave velocity predictions, enabling enhanced simulation and data analysis for Martian seismic studies.

- *Key Steps*:
  - *Data Generation using GAN*: Train a GAN to generate realistic Martian seismic data, including bulk modulus, shear modulus, and density. Ensure the generated values align with known Martian physical constraints for each geological layer (core, mantle, crust).
  - *Exploratory Data Analysis (EDA)*: Perform thorough EDA on the generated data to explore the distribution of features and relationships between them.
  - *Correlation Heatmap*: Generate a correlation heatmap to visualize relationships between key seismic features and better understand their interactions.
  - *Predicting Wave Velocities*: Use the generated data to predict P-wave and S-wave velocities for Martian seismic studies, ensuring realistic transitions between the crust, mantle, and core.
