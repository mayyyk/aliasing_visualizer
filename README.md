# Aliasing Visualizer

**Real-time interactive visualization of signal aliasing and DFT frequency domain effects**

---

## 📸 Demo

[streamlit-app-2026-01-18-12-01-89.webm](https://github.com/user-attachments/assets/407402f3-0f85-42fe-982f-a3b07c98c035)

---

## About

The **Aliasing Visualizer** is an interactive Streamlit application designed to demonstrate the relationship between sampling frequency, signal frequency, and the aliasing phenomenon in digital signal processing.  The tool provides synchronized time-domain and frequency-domain visualizations, allowing engineers and students to explore how violating the Nyquist-Shannon sampling theorem results in frequency aliasing.

The visualizer computes an idealized DFT representation showing DC offset (0 Hz bin) and AC signal components, with dynamic alias frequency calculation when the signal frequency exceeds the Nyquist limit.  Supports multiple waveform types and real-time parameter adjustment for educational and analysis purposes.

---

## Tech Stack

- **Python 3.x**
- **Streamlit** — Web application framework
- **NumPy** — Numerical computation and signal generation
- **Plotly** — Interactive plotting and visualization
- **Matplotlib** — Supporting visualization library

---

## Key Features

- **Dual-Domain Visualization**:  Simultaneous time-domain (analog signal + discrete samples) and frequency-domain (DFT spectrum) plots
- **Aliasing Detection**: Automatic identification and warning when signal frequency exceeds Nyquist frequency, with computed alias frequency display
- **Multi-Waveform Support**:  Sine, square, triangle, and sawtooth signal generation with configurable amplitude, frequency, and DC offset
- **Interactive Parameter Control**: Real-time adjustment of sampling frequency (1-2000 Hz), signal frequency (1-2000 Hz), amplitude, and DC offset via sidebar controls

---

## Installation/Usage

### Quick Start

```bash
# Clone the repository
git clone https://github.com/mayyyk/aliasing_visualizer.git
cd aliasing_visualizer

# Install dependencies
python3 -m venv venv
source venv/bin/activate
pip install -r requirements. txt

# Run the application
streamlit run app.py
```

Access the visualizer at `http://localhost:8501`

### Docker (Optional)

```bash
# If . devcontainer is configured
devcontainer open
```

---

## Configuration

Adjust parameters via the sidebar: 
- **DC Offset**: -5V to +5V
- **Amplitude**: 0 to 10V
- **Signal Shape**: sine | square | triangle | sawtooth
- **Signal Frequency**: 1-2000 Hz
- **Sampling Frequency**: 1-2000 Hz

---

**License**: MIT
**Author**: [@mayyyk](https://github.com/mayyyk)
