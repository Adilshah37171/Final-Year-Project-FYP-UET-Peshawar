# 4-Port MIMO Microstrip Patch Antenna for 5G Millimeter-Wave Applications

## Project Overview

This project presents the design, simulation, and performance evaluation of a compact 4-port MIMO microstrip patch antenna for 5G millimeter-wave applications operating at 28 GHz. The antenna is developed using CST Microwave Studio on a Rogers RT/duroid 5880 substrate, selected for its low dielectric loss and high-frequency stability. The design focuses on achieving high gain, wide bandwidth, strong isolation, and high radiation efficiency while maintaining a compact footprint suitable for modern wireless systems.ML Algorithm is used to predict the directivity of Antenna in oreder to reduce computational resrouces and time required for long simulations for such complex design in CST Software.

## Key Performance Parameters

Key performance parameters including S-parameters (S11), VSWR, gain, directivity, radiation efficiency, and radiation patterns are analyzed to validate the antenna's performance. The proposed design achieves:

- **High Isolation**: >29 dB between antenna elements
- **Low Envelope Correlation Coefficient (ECC)**
- **High Diversity Gain**
- Ensuring reliable and high-capacity communication in MIMO-based 5G systems

## Machine Learning Integration

In addition to conventional electromagnetic simulation, this project integrates machine learning techniques to enhance the antenna design process. Regression-based ML model Gradient Boost (XGBoost) is  trained on simulation data of 320 Iterations to predict  as directivity of the MIMO Antenna. This approach significantly reduces computational complexity and simulation time while maintaining high prediction accuracy.

## Methodology & Contribution

The combination of advanced antenna design and data-driven optimization demonstrates an efficient methodology for next-generation wireless system development. This work contributes toward improving design efficiency, performance optimization, and practical implementation of compact MIMO antennas for 5G communication systems.
**Step 1: Designing In CST Software**
Designed a single patch MSPA in CST
<img width="436" height="413" alt="image" src="https://github.com/user-attachments/assets/6bc667d1-7896-4b11-998b-c31278c47167" />
simulated and tested its performance,proceeded to dual patch-single feed design

<img width="172" height="123" alt="image" src="https://github.com/user-attachments/assets/71d09db0-4f6e-4248-90b4-7a435cfdb765" />


Then final design of 4-Port MIMO was designed.

<img width="439" height="433" alt="image" src="https://github.com/user-attachments/assets/8557d2d8-67e5-46d6-a23a-878fadad4c70" />
---------------------------------------------------------------------------------------------------------------------------------------------
<img width="525" height="534" alt="image" src="https://github.com/user-attachments/assets/4385ce36-1ac8-4efc-91cf-955b73c59db6" />

**Step 2:Data Set Collection**
We gathered a CSV file with 320 iterations of final design,each simulations took on average 3 hours to complete and give result for different parameters ,radiation patterns of design.

**Step 3:Model Training and Testing**
Trained XGBoost model on dataset and predicted its accuracy for prediction of directivity of antenna,it yielded 98.5% accuracy.


## Technologies Used

- **Simulation Tool**: CST Microwave Studio
- **Substrate**: Rogers RT/duroid 5880
- **Operating Frequency**: 28 GHz (5G mmWave)
- **Machine Learning**: Random Forest, Regression Models
- **Analysis**: S-parameters, VSWR, Gain, Directivity, Radiation Patterns

## Project Structure

```
Final-Year-Project-FYP-UET-Peshawar/
├── README.md
├── Simulation/
│   └── CST Microwave Studio Files
├── ML Models/
│   └── ML algorithms and training data
└── Results/
    └── Performance analysis and radiation patterns
```

## Author

**Syed Adil Shah**  
Final Year Project - University of Engineering and Technology (UET) Peshawar

## License
Subjected to demand/Permisible to use for research Work/Academic Practices.
