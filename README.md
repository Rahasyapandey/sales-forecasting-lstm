# 📈 AI-Based Sales Forecasting with LSTM
A deep learning approach to time-series forecasting, specifically designed to showcase advanced **Matplotlib** visualization techniques for GSoC 2026.

## 📊 Visualization Showcase
The core of this project is translating complex LSTM outputs into human-readable insights using high-fidelity plots.

<p align="center">
  <img src="demo_plot (3).png" width="800" alt="LSTM Sales Forecast Performance">
</p>

### 🎨 Matplotlib Technical Implementation
To meet the standards of the Matplotlib community, this project utilizes:
* **Custom Styling:** Applied the `ggplot` stylesheet for a professional, research-grade aesthetic.
* **Marker Logic:** Distinct markers (`o` for history, `s` for forecast) to differentiate between ground-truth and predicted data points.
* **Visual Hierarchy:** Used bolded titles, custom axis labeling, and high-DPI (300) rendering to ensure clarity across all screen sizes.
* **Forecast Continuity:** Implemented a seamless transition between historical and future arrays using `np.append` for a single-path visualization.

---

## 🧠 Model Architecture
This forecasting engine uses a **Long Short-Term Memory (LSTM)** network to identify seasonal patterns and trends:
* **Preprocessing:** `MinMaxScaler` normalization for stable gradient descent.
* **Layers:** 50-unit LSTM layer followed by a Dense output layer for point-wise prediction.
* **Optimizer:** Adam optimizer with Mean Squared Error (MSE) loss function.

---

## 🚀 GSoC 2026 & Matplotlib Integration
This repository serves as a technical precursor to my proposal for the **"Indirect Transforms"** project. 

**Why this matters:**
Understanding how data is mapped to the screen (the "Transform Pipeline") is crucial. By building this forecaster, I've explored:
1. How data coordinates map to pixel coordinates during real-time plotting.
2. The necessity of efficient rendering when dealing with large time-series datasets.
3. Customizing the `Axes` object to handle future-dated time-steps outside the original training range.

---

## 👤 Contact & GSoC 2026 Commitment

### 📮 Contact Information
* **Name:** Rahasya Pandey
* **Email:** rahasyapandey@gmail.com
* **Mobile/Chat:** +91 8849391872
* **Twitter:** [@RahasyaPandey](https://twitter.com/RahasyaPandey)
* **GitHub:** [Rahasyapandey](https://github.com/Rahasyapandey)
* **Zulip:** `@Rahasya_pandey` (Matplotlib Community)

### ⏳ Availability Statement
I am applying for the **Indirect Transforms** project. 
* **Weekly Commitment:** I am committed to dedicating **35-40 hours per week** to this project.
* **Other Commitments:** I have **no other internships, jobs, or conflicting academic courses** during the GSoC coding period (May – August 2026). This is my primary focus for the summer.

---

## 🛠️ Installation & Usage
```bash
git clone [https://github.com/Rahasyapandey/sales-forecasting-lstm.git](https://github.com/Rahasyapandey/sales-forecasting-lstm.git)
pip install -r requirements.txt
python sales_forecasting_lstm.py
