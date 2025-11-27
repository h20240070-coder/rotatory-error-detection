# Fault Detection in Rotary Electrical Machines 

## Project Overview

This project focuses on automatic fault detection in induction motors using a multimodal machine-learning approach. Motor signals generated from MATLAB/Simulink are segmented, converted into spectrogram images, and paired with numerical features such as RMS currents, THD, torque, speed, flux components, and slip. These combined datasets are used to train a hybrid CNN–MLP deep learning model that learns both visual frequency patterns and statistical signal information. The system provides reliable classification of faults such as Ground Insulation (GI), Stator Inter-Turn Short Circuit (SITSC), Broken Rotor Bar (BRB), BRB-Lite, and Unbalanced Voltage (UB), enabling early and accurate condition monitoring.

## Features

- Automated signal segmentation with overlap
- Spectrogram image generation
- Numerical feature extraction
- Multimodal dataset creation
- CNN + MLP hybrid architecture
- Fault classification (healthy, GI, SITSC, BRB, BRB-lite, UB)

  


