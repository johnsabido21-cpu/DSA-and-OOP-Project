# DSA-and-OOP-Project

# NEON STRIKE — Java Space Shooter Game

## 📌 Project Overview
**NEON STRIKE** is a fast‑paced 2D arcade space shooter built using Java Swing. The player controls a neon spaceship, shoots down incoming enemies, collects power‑ups, survives waves, and progresses through levels. This project demonstrates Object‑Oriented Programming (OOP) and Data Structures & Algorithms (DSA) concepts.

## 🎮 Features
✅ Player movement using W A S D
✅ Mouse aiming + left‑click shooting
✅ Multi‑shot power‑up system
✅ Three enemy types with different behaviors
✅ Particle explosion effects
✅ Level progression system
✅ Score, health, and level HUD
✅ Pause (ESC) + Restart (R)
✅ Screen shake on damage
✅ Dynamic enemy spawning that scales with level

## 🧠 OOP Concepts Used
- **Encapsulation**: Each class (Bullet, Enemy, Particle, PowerUp) stores its own position, health, color, and state.
- **Abstraction**: The main game loop calls high‑level methods such as `updateGame()`, `drawPlayer()`, `spawnEnemy()` without needing every rendering detail.
- **Composition**: The `SpaceShooter` class contains collections of bullets, enemies, particles, and power‑ups.
- **Polymorphism potential**: Although the original code does not use a formal parent `GameObject` class, each entity has its own `draw()` method which can be refactored for true polymorphism.

## 📊 DSA Concepts Used
- **`ArrayList`**: Stores dynamic lists of bullets, enemies, particles, and power‑ups.
  - Time complexity: Add ≈ O(1) amortized; iteration ≈ O(n); removal from middle ≈ O(n)
- **`Iterator`**: Safely removes objects during iteration to avoid `ConcurrentModificationException`.
- **Brute‑force collision detection**: Checks distance between bullets and enemies using Euclidean distance (O(B × E)).
- **Filtering / cleanup**: Removes dead or off‑screen objects each frame.
- **Spawn scheduling**: Uses a counter to trigger enemy spawning at variable intervals.

## 🕹️ Controls
- **W A S D**: Move spaceship
- **Mouse**: Aim
- **Left‑Click**: Shoot
- **ESC**: Pause / Resume
- **R**: Restart after game over

## 💻 How to Run
1. Save the full Java code as `NeonStrike.java`
2. Compile using:
   ```bash
   javac NeonStrike.java
   
