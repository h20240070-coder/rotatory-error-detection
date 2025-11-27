# Fault Detection in Rotary Electrical Machines ⚡🔧

A machine learning-based system for detecting electrical faults in induction motors using simulated time-series data from MATLAB/Simulink and spectrogram analysis.

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Machine Learning](https://img.shields.io/badge/Machine-Learning-orange)
![MATLAB](https://img.shields.io/badge/MATLAB-Simulink-red)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Latest-green)
![Status](https://img.shields.io/badge/Status-Completed-success)

---

## 📖 Table of Contents
- [Overview](#overview)
- [Project Structure](#project-structure)
- [Dataset](#dataset)
- [Methodology](#methodology)
- [Key Features](#key-features)
- [Tech Stack](#tech-stack)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [Future Enhancements](#future-enhancements)
- [Contributing](#contributing)
- [License](#license)

## 🚀 Overview

This project implements an intelligent fault detection system for 3-phase induction motors using electrical signal analysis and machine learning. The system identifies different severity levels of electrical faults based on simulated voltage, current characteristics and spectrogram analysis.

**Fault Types Detected:**
- **Healthy Operation** ✅ - Normal motor operation (384 samples)
- **10Ω Electrical Fault** ⚠️ - Mild fault condition
- **30Ω Electrical Fault** 🚨 - Moderate fault condition  
- **60Ω Electrical Fault** 🔥 - Severe fault condition

## 📁 Project Structure
rotatory-error-detection/
├── ml_for_ee_project (1).ipynb # Main Jupyter Notebook with ML analysis
├── MATLAB Simulation Files/
│ ├── AC_Voltage_Control_3phase_IM.slx # Main Simulink 3-phase motor model
│ ├── healthy_dataset_generation_script.mlx # Healthy data generation
│ └── rotor_fault_generation_script.mlx # Faulty data generation
├── Spectrogram Datasets/
│ ├── spectrograms_healthy/ # Healthy motor spectrograms
│ ├── spectrograms_faulty_10ohm/ # 10Ω fault spectrograms
│ ├── spectrograms_faulty_30ohm/ # 30Ω fault spectrograms
│ └── spectrograms_faulty_60ohm/ # 60Ω fault spectrograms
├── Results/ # Generated results and plots
└── README.md # Project documentation


## 📊 Dataset

### Simulation Details
- **Tool Used**: MATLAB Simulink & Live Scripts
- **Model**: 3-phase AC Voltage Control Induction Motor
- **Signals**: Voltage and Current time-series responses
- **Visualization**: Spectrogram analysis for frequency-time domain features

### Class Distribution & Data Generation
- **Healthy Samples**: 384 (generated via `healthy_dataset_generation_script.mlx`)
- **Faulty Samples**: 100 each for 10Ω, 30Ω, and 60Ω faults (via `rotor_fault_generation_script.mlx`)
- **Total Samples**: 684 time-series recordings

### Spectrogram Analysis
Each class has dedicated spectrogram folders containing time-frequency representations:
- `spectrograms_healthy/` - Normal operation patterns
- `spectrograms_faulty_10ohm/` - Mild fault characteristics
- `spectrograms_faulty_30ohm/` - Moderate fault patterns
- `spectrograms_faulty_60ohm/` - Severe fault signatures

## 🔬 Methodology

### 1. Simulation Phase (MATLAB/Simulink)
- Developed 3-phase induction motor model in `AC_Voltage_Control_3phase_lM.slx`
- Generated healthy data using `healthy_dataset_generation_script.mlx`
- Simulated rotor electrical faults (10Ω, 30Ω, 60Ω) using `rotor_fault_generation_script.mlx`
- Collected voltage and current time-series data under varying conditions

### 2. Signal Processing & Feature Extraction
- **Time-domain analysis**: Statistical features from raw signals
- **Frequency-domain analysis**: Spectrogram generation for time-frequency analysis
- **Feature engineering**: Extraction of discriminative patterns from spectrograms

### 3. Machine Learning Pipeline (Jupyter Notebook)
- Data preprocessing and normalization
- Feature selection and importance analysis
- Model training with cross-validation
- Performance evaluation of multiple classifiers

## ✨ Key Features

- **Electrical Fault Detection** ⚡ - Identifies resistance-based faults in motor windings
- **Multi-class Classification** 🎯 - Distinguishes between 4 different operational states
- **Spectrogram Analysis** 📊 - Time-frequency domain feature extraction
- **High Accuracy** 📈 - Achieves 91% accuracy with Random Forest
- **Comprehensive Simulation** 🔬 - Based on detailed MATLAB/Simulink 3-phase motor model
- **Realistic Fault Modeling** 🎭 - Accurate simulation of different fault severities

## 🛠️ Tech Stack

### Core Technologies
- **Python 3.8+** with Jupyter Notebook - ML analysis and modeling
- **MATLAB/Simulink** - Motor simulation and data generation
- **MATLAB Live Scripts** - Interactive data generation scripts
- **Scikit-learn** - Machine learning algorithms

### Machine Learning Models
- **Random Forest Classifier** - Primary model (91% accuracy)
- **Support Vector Machines (SVM)** - Comparative model (86% accuracy)

### Signal Processing
- **Spectrogram Analysis** - Time-frequency representations
- **Statistical Feature Extraction** - From time-series data
- **Signal Preprocessing** - Filtering and normalization

## 📥 Installation & Setup

### Prerequisites
- Python 3.8+ with Jupyter Notebook
- MATLAB (for simulation files, optional)
- Required Python packages

### Python Environment Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/h20240070-coder/rotatory-error-detection.git
   cd rotatory-error-detection

   
## 📊 Dataset

### Simulation Details
- **Tool Used**: MATLAB Simulink & Live Scripts
- **Model**: 3-phase AC Voltage Control Induction Motor
- **Signals**: Voltage and Current time-series responses
- **Visualization**: Spectrogram analysis for frequency-time domain features

### Class Distribution & Data Generation
- **Healthy Samples**: 384 (generated via `healthy_dataset_generation_script.mlx`)
- **Faulty Samples**: 100 each for 10Ω, 30Ω, and 60Ω faults (via `rotor_fault_generation_script.mlx`)
- **Total Samples**: 684 time-series recordings

### Spectrogram Analysis
Each class has dedicated spectrogram folders containing time-frequency representations:
- `spectrograms_healthy/` - Normal operation patterns
- `spectrograms_faulty_10ohm/` - Mild fault characteristics
- `spectrograms_faulty_30ohm/` - Moderate fault patterns
- `spectrograms_faulty_60ohm/` - Severe fault signatures

## 🔬 Methodology

### 1. Simulation Phase (MATLAB/Simulink)
- Developed 3-phase induction motor model in `AC_Voltage_Control_3phase_lM.slx`
- Generated healthy data using `healthy_dataset_generation_script.mlx`
- Simulated rotor electrical faults (10Ω, 30Ω, 60Ω) using `rotor_fault_generation_script.mlx`
- Collected voltage and current time-series data under varying conditions

### 2. Signal Processing & Feature Extraction
- **Time-domain analysis**: Statistical features from raw signals
- **Frequency-domain analysis**: Spectrogram generation for time-frequency analysis
- **Feature engineering**: Extraction of discriminative patterns from spectrograms

### 3. Machine Learning Pipeline (Jupyter Notebook)
- Data preprocessing and normalization
- Feature selection and importance analysis
- Model training with cross-validation
- Performance evaluation of multiple classifiers

## ✨ Key Features

- **Electrical Fault Detection** ⚡ - Identifies resistance-based faults in motor windings
- **Multi-class Classification** 🎯 - Distinguishes between 4 different operational states
- **Spectrogram Analysis** 📊 - Time-frequency domain feature extraction
- **High Accuracy** 📈 - Achieves 91% accuracy with Random Forest
- **Comprehensive Simulation** 🔬 - Based on detailed MATLAB/Simulink 3-phase motor model
- **Realistic Fault Modeling** 🎭 - Accurate simulation of different fault severities

## 🛠️ Tech Stack

### Core Technologies
- **Python 3.8+** with Jupyter Notebook - ML analysis and modeling
- **MATLAB/Simulink** - Motor simulation and data generation
- **MATLAB Live Scripts** - Interactive data generation scripts
- **Scikit-learn** - Machine learning algorithms

### Machine Learning Models
- **Random Forest Classifier** - Primary model (91% accuracy)
- **Support Vector Machines (SVM)** - Comparative model (86% accuracy)

### Signal Processing
- **Spectrogram Analysis** - Time-frequency representations
- **Statistical Feature Extraction** - From time-series data
- **Signal Preprocessing** - Filtering and normalization

## 📥 Installation & Setup

### Prerequisites
- Python 3.8+ with Jupyter Notebook
- MATLAB (for simulation files, optional)
- Required Python packages

### Python Environment Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/h20240070-coder/rotatory-error-detection.git
   cd rotatory-error-detection
2.Install required packages
  pip install numpy pandas scikit-learn matplotlib seaborn scipy jupyter

3.Launch Jupyter Notebook

## MATLAB Setup (Optional - for simulation)

1.Open MATLAB

2.Navigate to project directory

3.Open AC_Voltage_Control_3phase_lM.slx to view the motor model

4.Run Live Scripts for data generation

## 🎯 Usage

**Running the ML Analysis**

1.Open ml_for_ee_project (1).ipynb in Jupyter Notebook

2.**Run cells sequentially to**:

  Load and preprocess spectrogram data
  
  Extract features from time-series signals
  
  Train machine learning models
  
  Evaluate model performance
  
  Generate results and visualizations
