# 🤖 Brownian Motion Robot Simulation

This project implements and visualizes **Brownian Motion** behavior in a robot using Python and `matplotlib`. It was created as part of a [GSoC 2025](https://summerofcode.withgoogle.com/) application challenge under the robotics and simulation domain.

---

## 🧠 Problem Statement

> **Simulate a robot that mimics Brownian Motion in a confined 2D arena using only the Python standard library and NumPy.**

Brownian Motion is the **random movement of particles in a fluid**, caused by collisions with other fast-moving molecules. In robotics, this behavior is often useful for:

- **Swarm robotics**
- **Random exploration**
- **Environmental coverage**

This project simulates a **robot as a point** in a 2D space, which:
- Moves continuously in a direction
- On **collision with boundaries**, it rotates randomly
- Then resumes forward motion in the new direction

---

## 🎯 Objectives

- ✅ Build a Python module (`robot.py`) to simulate Brownian behavior
- ✅ Visualize robot movement using `matplotlib`
- ✅ Export the simulation as a `.gif` file
- ✅ Avoid third-party libraries (except `matplotlib` and `numpy`)

---

## 🧪 How It Works

- The robot starts at the **center** of a square arena (500x500 units).
- It moves in a straight line with a constant speed.
- When it hits a wall (boundary), it:
  - **Bounces off** by turning a random angle (30°–150°)
  - Continues forward in that new direction
- This mimics **chaotic Brownian movement**.

---

## 💻 Run It Yourself

### 📦 Requirements

- Python 3.x
- `numpy`
- `matplotlib`
- `pillow` (for saving gifs)

```bash
pip install numpy matplotlib pillow
