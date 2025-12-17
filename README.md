# 👁️ OmniScout

![Version](https://img.shields.io/badge/version-1.0-blue?style=for-the-badge)
![License](https://img.shields.io/badge/license-CC_BY--NC_4.0-red?style=for-the-badge)
![Status](https://img.shields.io/badge/status-active-success?style=for-the-badge)

> **A robust, client-side reconnaissance dashboard designed to analyze and visualize browser fingerprinting capabilities and Web APIs.**

---

## 📖 About The Project

**OmniScout** is a technical demonstration and research tool developed to explore the depth of data available to websites through modern browser APIs. Unlike standard analytics tools, OmniScout dives deep into hardware inspection, network sniffing, and sensor data.

The project demonstrates the difference between **Passive Fingerprinting** (data available immediately upon page load) and **Active Reconnaissance** (data requiring user interaction or permissions).

### 🎯 Objectives

* **Educational:** To demonstrate how much information is exposed by default in modern web browsers.
* **Security Research:** To test browser privacy settings, VPN leaks, and extension blocking capabilities.
* **JS Vanilla Power:** To showcase advanced DOM manipulation and API integration without external dependencies.

---

## ⚡ Features

### 🔍 Passive Gathering (Automatic)

* **Core Identity:** User Agent parsing, platform detection, and browser engine analysis.
* **Hardware Inspection:** * CPU Concurrency & RAM estimation.
    * **GPU Fingerprinting:** Extracts exact Graphics Card Vendor and Renderer via WebGL.
* **Network Intelligence:**
    * **Connection type** (4G/WiFi) and Downlink speed estimation.
    * **Public IP Address** fetching (via external API).
* **Battery Status:** Real-time charging monitoring and level detection.
* **Screen Metrics:** High-precision display analysis including pixel depth and orientation.

### ⚠️ Active Reconnaissance (Trigger-Based)

* **WebRTC Leak Test:** Attempts to extract the local LAN IP address via ICE Candidates, bypassing proxies in some configurations.
* **Geolocation:** Requests high-accuracy GPS coordinates, altitude, and speed.
* **Media Enumeration:** Scans and lists exact model names of connected Cameras and Microphones.
* **Sensor Access:** Real-time reading of Gyroscope and Accelerometer data (Mobile).
* **Clipboard & Haptics:** Tests access to system clipboard and vibration motors.

---

## 🛠️ Technologies Used

This project is built with a "Zero-Dependency" philosophy to ensure maximum speed and transparency.

* **HTML5:** Semantic structure and API integration.
* **CSS3:** Custom "Dark Glass" UI (Glassmorphism), CSS Grid, and Flexbox. **No Bootstrap or Frameworks used.**
* **Vanilla JavaScript (ES6+):**
    * `Navigator API`
    * `WebGL API` (for GPU info)
    * `WebRTC API` (RTCPeerConnection for IP leaks)
    * `Geolocation API`
    * `Battery Status API`
    * `MediaDevices API`

---

## 🚀 How to Run

Since OmniScout relies purely on client-side technologies, it does not require a backend server for the core logic (except for the Public IP fetch).

1.  **Clone the repository:**
    [code-block]bash
    git clone https://github.com/rubensbraz/OmniScout.git
    [code-block]

2.  **Open the file:**
    Simply navigate to the folder and open `index.html` in any modern web browser.

    > **Note:** Some features (like Geolocation and Sensors) require a **Secure Context (HTTPS)** or `localhost` to function correctly due to modern browser security policies.
---

## 📄 License

This project is licensed under the **Creative Commons Attribution-NonCommercial 4.0 International (CC BY-NC 4.0)**.

### You are free to:
* **Share** — copy and redistribute the material in any medium or format.
* **Adapt** — remix, transform, and build upon the material.

### Under the following terms:
* **Attribution** — You must give appropriate credit to **Rubens Braz**, provide a link to the license, and indicate if changes were made.
* **NonCommercial** — You may not use the material for commercial purposes.

[View Full License](https://creativecommons.org/licenses/by-nc/4.0/)

---

## 👨‍💻 Author

**[Rubens Braz](https://rubensbraz.com/)**
