🌟 Project Overview
This repository contains the WESAD Future Stress Dataset, a feature‑engineered multimodal physiological dataset designed for stress detection and prediction using wearable sensors. It includes raw signals (ACC, BVP, EDA, TEMP, HR) and advanced derived features such as HRV metrics, rolling‑window statistics, slopes, and lagged values.

This dataset is ideal for machine learning models focused on stress classification, continuous stress prediction, and real‑time wearable‑health analytics.


Full Feature Breakdown
🕒 timestamp
Time index for each sample.

🏃 Accelerometer (ACC)
Raw motion signals from the wearable.

acc_x, acc_y, acc_z — 3‑axis acceleration

acc_magnitude — 
𝑥
2
+
𝑦
2
+
𝑧
2
, overall movement intensity

acc_magnitude_mean_60s — 60‑second rolling mean

acc_magnitude_slope_60s — trend over the last 60 seconds

acc_magnitude_lag_5s, acc_magnitude_lag_10s — movement 5–10 seconds earlier

These help detect physical activity vs. rest, which is crucial for stress modeling.

❤️ Blood Volume Pulse (BVP)
bvp — raw PPG signal used to derive HR and HRV.

💓 Heart Rate & HRV
hr — instantaneous heart rate

ibi — inter‑beat interval

hrv_rmssd — RMSSD, a parasympathetic HRV metric

hrv_sdnn — SDNN, overall HRV variability

hr_mean_60s — rolling mean HR

hr_slope_60s — HR trend

hr_lag_5s, hr_lag_10s — HR from 5–10 seconds earlier

HRV is one of the strongest indicators of stress.

🫁 Respiration
resp_rate — breaths per minute (likely derived from chest expansion or PPG).

🧊 Temperature
temp — skin temperature

temp_mean_60s — rolling mean

temp_slope_60s — trend
Temperature often drops during stress due to vasoconstriction.

🧪 Electrodermal Activity (EDA)
eda — raw skin conductance

eda_peaks — number of SCR peaks

eda_mean_60s — rolling mean

eda_slope_60s — trend

eda_lag_5s, eda_lag_10s — lagged EDA values

EDA is the most direct measure of sympathetic arousal.

🔁 Lag Features (5s, 10s)
These capture short‑term temporal dynamics:

hr_lag_5s, hr_lag_10s

eda_lag_5s, eda_lag_10s

acc_magnitude_lag_5s, acc_magnitude_lag_10s

Lag features help models detect rising or falling physiological trends.

🧩 What This Dataset Is Designed For
This feature set is ideal for:

Stress classification (baseline vs. stress vs. amusement)

Continuous stress prediction

Personalized stress modeling

Multimodal physiological analysis

Real‑time wearable‑health AI 

It includes raw signals + engineered features, which is exactly what modern stress‑prediction models use.

🤝 Contributing
Pull requests are welcome.
For major changes, please open an issue first to discuss what you’d like to modify.

📄 License
MIT License

📬 Contact
For questions or collaboration, feel free to reach out.
