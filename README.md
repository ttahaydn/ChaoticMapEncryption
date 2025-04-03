
# 🔐 Secure IoT Health Data Transmission via Chaotic Encryption

This project explores and compares four different chaotic encryption methods to secure the transmission of chest tomography images in IoMT (Internet of Medical Things) systems. It includes both algorithm implementation (in Python) and secure transmission simulation (in OMNET++).

## 📌 Project Objective

To evaluate and compare the performance of various chaotic encryption algorithms in terms of:

- **Security** (Entropy, Correlation, Key Sensitivity, etc.)
- **Image Quality** (PSNR, SSIM)
- **Computational Efficiency**
- **Resistance to Attacks** (NPCR, UACI, EDR)

The most optimal algorithm (3D Lorenz Attractor) is then used for a secure transmission simulation in an IoMT environment using **OMNET++**.

## 🔬 Chaotic Encryption Methods Implemented

| Method           | Dimensions | Description                                           |
|------------------|------------|-------------------------------------------------------|
| Logistic Map     | 1D         | Simple and fast, uses XOR-based pixel modification   |
| Henon Map        | 2D         | Employs chaotic pixel rearrangement                  |
| Lorenz Attractor | 3D         | Strong entropy and structural preservation           |
| Chen Map         | 4D         | High NPCR but high overhead and lower entropy        |

## 🧪 Evaluation Metrics

- **Entropy**
- **Correlation**
- **PSNR (Peak Signal-to-Noise Ratio)**
- **SSIM (Structural Similarity Index)**
- **NPCR / UACI**: Differential attack resistance
- **EDR (Edge Difference Rate)**
- **Key Sensitivity**

## 🛠️ Tools & Technologies

- 🐍 **Python**: For algorithm implementation and performance analysis  
  Libraries used: `NumPy`, `OpenCV`, `Matplotlib`
  
- 🖥️ **OMNET++**: For simulating secure IoMT data transmission

## 🧠 Summary of Results

| Metric             | Logistic | Henon   | Lorenz  | Chen    |
|--------------------|----------|---------|---------|---------|
| Entropy            | 7.9693   | 7.9987  | 7.9998  | 6.9960  |
| Correlation        | 0.1228   | -0.0889 | 0.7638  | 0.9971  |
| PSNR               | 6.91     | 8.23    | 8.12    | 5.47    |
| SSIM               | 0.0056   | 0.0092  | 0.0098  | 0.1249  |
| NPCR (%)           | 99.80    | 99.63   | 99.59   | 99.95   |
| UACI (%)           | 46.84    | 50.29   | 50.15   | 40.22   |
| Key Sensitivity (%)| 99.21    | 99.58   | 99.54   | 0.0037  |
| Time (s)           | 0.63     | 0.80    | 0.83    | 2.55    |

**✅ Best Overall Performance:** Henon Map & Lorenz Attractor  
**✅ Best for Transmission Simulation:** Lorenz Attractor (used in OMNET++)

## 🚀 Getting Started

### 🔧 Requirements

- Python 3.x
- OMNET++ (version used in the project)
- Required Python packages:
```bash
pip install numpy opencv-python matplotlib
```

## 👨‍💻 Authors

- Hasan Uslu 
- Umut Öztürk  
- Abdullah Taha Aydın  
  
Eskisehir Osmangazi University – Computer Engineering

## 📚 References

This project is based on and compares the methods presented in the following academic papers and surveys. Full citation list is available in `Report.pdf`.
