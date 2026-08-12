## QuantumCanvas

A lightweight Python utility for visualizing mathematical quantum mechanical wave functions and their probability densities.

## 🚀 Features

- **Wave Function Visualization**: Easily plot the real and imaginary components of complex-valued wave functions.
- **Probability Density**: Automatically calculates and shades the area for $|\psi(x)|^2$.
- **Customizable Ranges**: Flexible spatial domain and resolution support using NumPy and Matplotlib.
- **Educational Tool**: Ideal for visualizing common quantum states like the Harmonic Oscillator or moving Gaussian wave packets.

## 📋 Usage

To use the `QuantumCanvas`, define a wave function $\psi(x)$ and pass it to the plotting methods:

```python
import numpy as np
from quantum_canvas import QuantumCanvas

# Define your wave function
def my_psi(x):
    return np.exp(-x**2)

# Initialize and plot
canvas = QuantumCanvas(x_range=(-5, 5))
canvas.plot_wavefunction(my_psi, label='\psi')
canvas.plot_probability_density(my_psi)
```

## 📝 Examples Included

- **Harmonic Oscillator**: Visualizing the ground state $\psi_0$.
- **Gaussian Wave Packet**: Visualizing moving states with complex phase factors $e^{ikx}$.

## 🛠️ Requirements

- NumPy
- Matplotlib
