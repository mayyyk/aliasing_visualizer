# Aliasing & DFT Visualizer

**Real-time interactive visualization of signal aliasing effects and Discrete Fourier Transform behavior in sampled systems.**

---

## 📊 GIF/Screenshot

_[Interactive dashboard preview - add screenshot here]_

---

## About

The Aliasing Visualizer is an educational web application that demonstrates the fundamental concepts of digital signal processing, specifically how sampling rate affects signal representation and introduces aliasing artifacts. The tool provides simultaneous time-domain and frequency-domain visualizations, allowing engineers and students to experiment with various signal parameters (DC offset, amplitude, frequency, waveform shape) and observe how insufficient sampling rates cause frequency components to be misrepresented in the discrete spectrum. This addresses the common learning challenge of understanding the Nyquist-Shannon sampling theorem through interactive experimentation rather than static diagrams.

---

## Tech Stack

- **Python 3.x** - Core runtime
- **Streamlit** - Interactive web framework
- **NumPy** - Numerical computation and signal generation
- **Plotly** - Interactive graphing and visualization
- **Matplotlib** - Additional plotting support

---

## Key Features

- **Interactive Signal Generation**: Configure DC offset, amplitude, frequency (1-2000 Hz), and waveform shape (sine, square, triangle, sawtooth) through an intuitive sidebar interface.

- **Dual-Domain Visualization**: Simultaneous rendering of time-domain signals (analog waveform with overlaid digital samples) and frequency-domain spectrum (ideal DFT representation with Nyquist frequency marker).

- **Real-Time Aliasing Detection**: Automatic calculation and visual indication when signal frequency exceeds Nyquist limit, displaying the aliased frequency bin and warning messages.

- **Educational Feedback**: Dynamic success/warning messages explain sampling correctness and aliasing behavior based on current parameter settings.

---

## Installation/Usage

```bash
# Clone the repository
git clone https://github.com/mayyyk/aliasing_visualizer.git
cd aliasing_visualizer

# Install dependencies
pip install -r requirements.txt

# Run the application
streamlit run app.py
```

Access the web interface at `http://localhost:8501` and adjust parameters in the sidebar to explore different signal scenarios.

---

_Built for DSP education and signal analysis exploration._
