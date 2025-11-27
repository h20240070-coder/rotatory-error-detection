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

## Results
- RandomForest
  <img width="662" height="550" alt="image" src="https://github.com/user-attachments/assets/64efd03f-4aa7-454d-b7ba-c52a8d917326" />

- Support Vector Machine
  <img width="659" height="551" alt="image" src="https://github.com/user-attachments/assets/8db90326-b1bc-45ff-b53d-1827dc6714be" />

- CNN
  ![WhatsApp Image 2025-11-27 at 18 53 19](https://github.com/user-attachments/assets/93867f16-6e91-467d-86b6-a0008f06e10a)



  


