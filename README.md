# ECG-Noise-Removal-using-FIR-Low-Pass-Filter
design and application of a low-pass FIR (Finite Impulse Response) filter to remove noise from an assumed electrocardiogram (ECG) signal

# ECG Signal Denoising using FIR Low-Pass Filter

This MATLAB project demonstrates the use of a **Finite Impulse Response (FIR) low-pass filter** to remove high-frequency noise from an assumed electrocardiogram (ECG) signal. The filter is designed using the **Hanning window method** and applied to a synthetic ECG signal composed of sinusoidal components and Gaussian noise.

---

## 📌 Features

- FIR filter design using windowing technique (Hanning window)
- Filtering of noisy ECG signal
- Time-domain and frequency-domain visualizations
- Analysis using periodograms and frequency response plots

---

## 🧠 Algorithm & Parameters

- **Sampling Frequency (Fs):** 1000 Hz  
- **Passband Frequency:** 50 Hz  
- **Stopband Frequency:** 150 Hz  
- **Passband Ripple:** 0.5 dB  
- **Stopband Attenuation:** 40 dB  
- **Filter Order (M):** 217  
- **Window Function:** Hanning  

---

## 🔬 Signal Generation

A synthetic ECG-like signal is generated as follows:
```matlab
ecg_signal = 0.7*sin(2*pi*10*t) + 0.5*sin(2*pi*30*t) + randn(size(t));

This signal simulates clean ECG components with added high-frequency noise.

# How the Filter Works
Compute normalized frequency bounds.

Define an ideal rectangular response.

Apply Hanning window to reduce spectral leakage.

Normalize the filter coefficients.

Filter the ECG signal using filter().

![image](https://github.com/user-attachments/assets/39aede99-a895-4ba3-b95d-9e393fe06bfe)
![image](https://github.com/user-attachments/assets/5740a8d1-8c51-4012-ab1f-8b8e9f08a8c1)
![image](https://github.com/user-attachments/assets/8b4ce15a-3174-43bd-b7c6-d9668a67271b)







