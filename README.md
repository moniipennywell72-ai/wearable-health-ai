# wearable-health-ai
Physiological feature extraction from SetA + SetB datasets
A unified pipeline for extracting physiological features from two multimodal wearable‑sensor datasets (SetA and SetB).
This project processes BVP, EDA/GSR, EMG, Respiration, Temperature, and Accelerometer signals, producing a clean, machine‑learning‑ready dataset: combined_features.csv.

⭐Key Features**
HRV extraction (RMSSD, SDNN, pNN50)
EDA/GSR peak detection + tonic level
EMG RMS, variance, peak amplitude
Respiration rate + amplitude
Temperature trend features
Accelerometer magnitude + variance
Safe handling of missing signals
Final merged dataset for ML workflows

📂 Project Structure
project/
│
├── setab.ipynb               # Main processing notebook
├── combined_features.csv     # Final merged dataset (SetA + SetB)
├── SetA_features.csv         # Extracted features from SetA
├── data.csv                  # Optional intermediate file
│
├── SetA/                     # Raw SetA .mat files
└── SetB/                     # Raw SetB .mat files



🧠 Dataset Overview
**SetA**
Daily recordings with 8 channels each:
ACC (acc_1 … acc_8)
TEMP (temp_1 … temp_8)
EDA (eda_1 … eda_8)
HR (hr_1 … hr_8)
**SetB**
Multi‑subject physiological recordings:
BVPr (raw BVP)
BVPw (windowed BVP)
EMGj (EMG)
GSR (EDA)
RESPr (respiration)
Not all subjects have all signals — missing data is handled safely.

🧪 Feature Extraction Summary
**HRV**
RMSSD
SDNN
pNN50
**EDA / GSR**
Tonic level
Number of peaks
Peak amplitude
**EMG**
RMS
Variance
Peak amplitude
**Respiration**
Estimated breath count
Amplitude
**Temperature**
Mean
Slope
Variance
**Accelerometer**
Magnitude
Variance

📈 Output File
combined_features.csv
Contains:
All SetA features
All SetB features
Subject IDs
Day labels
Source file names
Cleaned physiological metrics
This dataset is ready for:
Stress detection
Activity recognition
ML model training
Visualization
Statistical analysis

🤝 Contributing
Pull requests are welcome.
For major changes, please open an issue first to discuss what you’d like to modify.

📄 License
MIT License

📬 Contact
For questions or collaboration, feel free to reach out.
