# wearable-health-ai
Physiological feature extraction from SetA + SetB datasets
A unified pipeline for extracting physiological features from two multimodal wearable‑sensor datasets (SetA and SetB).
This project processes BVP, EDA/GSR, EMG, Respiration, Temperature, and Accelerometer signals, producing a clean, machine‑learning‑ready dataset: combined_features.csv.
**Key Features**
HRV extraction (RMSSD, SDNN, pNN50)
EDA/GSR peak detection + tonic level
EMG RMS, variance, peak amplitude
Respiration rate + amplitude
Temperature trend features
Accelerometer magnitude + variance
Safe handling of missing signals
Final merged dataset for ML workflows
