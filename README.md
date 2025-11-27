# Fault Detection in Rotary Electrical Machines 


This project focuses on detecting and classifying induction motor faults by using a multimodal machine-learning approach. The motor signals from Simulink are segmented, converted into spectrogram images, and combined with numerical features such as RMS currents, torque, speed, flux, and slip. These multimodal datasets are then used to train a hybrid CNN–MLP model capable of learning both visual and statistical patterns. By merging image-based frequency information with meaningful signal features, the system achieves robust classification of faults such as GI, SITSC, BRB, BRB-lite, and UB, enabling early and reliable fault diagnosis.


