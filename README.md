# Xiaomi Refresh Rate Controller

[![Platform](https://img.shields.io/badge/Platform-Android%2014%2B-green.svg)](https://developer.android.com/)
[![OS](https://img.shields.io/badge/OS-Xiaomi%20HyperOS-orange.svg)](https://www.mi.com/global/)
[![Tech Stack](https://img.shields.io/badge/UI-Jetpack%20Compose%20%7C%20Material%203-blue.svg)](https://developer.android.com/jetpack/compose)
[![Access](https://img.shields.io/badge/Permission-Root%20(Magisk%20%2F%20KernelSU%20%2F%20APatch)-red.svg)](https://github.com/topjohnwu/Magisk)

A root-powered refresh rate management tool tailored specifically for the **Xiaomi Pad 7** (and compatible HyperOS / MIUI devices). It allows users to lock refresh rates (144Hz, 120Hz, 90Hz, 60Hz, 48Hz, 30Hz), disable Joyose throttling, and switch rates directly from the **Control Center / Quick Settings** via a floating overlay.

---

## ✨ Features

- **🚀 Complete Refresh Rate Control:**
  - **144Hz (Peak Fluidity):** Locks max refresh rate for competitive gaming, fast UI response, and low stylus latency.
  - **120Hz (Smooth Performance):** Excellent balance between high frame rates and battery draw.
  - **90Hz (Balanced):** Silky scrolling with significantly better battery life than 144Hz.
  - **60Hz (Standard Saver):** Balanced everyday efficiency.
  - **48Hz (Cinema Mode):** Exact 2x cadence for 24fps movies and videos without pulldown judder.
  - **30Hz (Ultra Power Saver):** Cuts display controller power draw for reading books, documents, manga, or PDFs.

- **🎛️ Control Center Quick Tile with Floating Options:**
  - Tap the **Refresh Rate** Quick Settings tile from anywhere (in any app or game) to open a floating modal dialog.
  - Select any supported rate or revert to default in 1 tap without opening the full app.

- **⚡ Joyose FPS Uncap Toggle:**
  - Temporarily bypasses or disables `com.xiaomi.joyose` throttling profiles to maintain stable frame rates in games and heavy applications.

- **🔄 Auto-Apply on Boot:**
  - Automatically restores your preferred refresh rate and Joyose state after every system reboot.

- **🛡️ 1-Tap Reset to HyperOS Defaults:**
  - Instantly clears all root overrides (`min_refresh_rate`, `peak_refresh_rate`, `user_refresh_rate`) and returns the tablet to stock dynamic adaptive mode.

- **📱 Hardware-Aware Mode Detection:**
  - Queries `DisplayManager` directly to read native display modes supported by the panel.

---

## 📋 Requirements

1. **Device:** Xiaomi Pad 7 (or any Xiaomi / HyperOS / Android 14+ device with a high-refresh display).
2. **Root Access:** [Magisk](https://github.com/topjohnwu/Magisk), [KernelSU](https://github.com/tiann/KernelSU), or [APatch](https://github.com/bmax121/APatch).
3. **Android Version:** Android 13 or Android 14+ (HyperOS).

---

## 📥 Installation

1. Download the latest `pad-refresh-rate.apk` from the Releases section.
2. Install the APK on your device.
3. Open the app and grant **Superuser / Root** permission when prompted.
4. (Optional) Edit your **Quick Settings / Control Center** tiles and drag the **Refresh Rate** tile into your active tiles.

---

## 🛠️ Building from Source

### Prerequisites
- [Android Studio](https://developer.android.com/studio) (Koala / Ladybug or newer)
- JDK 17 or JDK 21
- Android SDK (API 34 / 35)

### Build Steps

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/xiaomi-pad-refresh-rate.git
   cd xiaomi-pad-refresh-rate
