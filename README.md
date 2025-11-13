# 🦠 SIR Epidemic Spread Simulation

![VirusGIF](https://media.giphy.com/media/l3vR1Xxv2zZkk0r0Q/giphy.gif)

The **SIR (Susceptible–Infected–Recovered)** model is a classic epidemiological framework that helps us understand how infectious diseases spread through a population.

This project implements the SIR model in **Python** using `NumPy`, `SciPy`, `Matplotlib`, and `Seaborn` to visualize how infections evolve over time.

---

## 📊 Model Overview

| Compartment | Description |
|--------------|--------------|
| 🧍‍♂️ **S (Susceptible)** | Individuals who can contract the disease |
| 🤒 **I (Infected)** | Individuals currently infected and spreading the disease |
| 💪 **R (Recovered)** | Individuals who have recovered and are immune |

---

## 🧮 Differential Equations

The model uses the following system of equations:

\[
\frac{dS}{dt} = -\beta SI
\]
\[
\frac{dI}{dt} = \beta SI - \gamma I
\]
\[
\frac{dR}{dt} = \gamma I
\]

Where:
- **β (beta)** → Infection rate  
- **γ (gamma)** → Recovery rate  

---

## ⚙️ Parameters Used
| Parameter | Meaning | Value |
|------------|----------|-------|
| `S0` | Initial susceptible population | 0.99 |
| `I0` | Initial infected population | 0.01 |
| `R0` | Initial recovered population | 0.0 |
| `β` | Transmission rate | 0.35 |
| `γ` | Recovery rate | 0.10 |
| `t` | Time (in days) | 0–160 |

---

## 🧰 Technologies Used
- **Python**
- **NumPy**
- **SciPy**
- **Matplotlib**
- **Seaborn**

---

## 🖼️ Simulation Output

The plot below shows the change in population proportions over time:

- 🔵 **Susceptible** – decreases as infection spreads  
- 🔴 **Infected** – rises and falls as the epidemic peaks and declines  
- 🟢 **Recovered** – increases as individuals recover  

![SIRChart](https://media.giphy.com/media/fAnEC88LccN7a/giphy.gif)

---

## 💻 Run the Code

```bash
python sir_model_simulation.py
