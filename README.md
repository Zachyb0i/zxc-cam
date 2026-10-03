# ZXC CAM 🚀❄️

> **The next-generation, lightweight PC hardware & thermal telemetry suite.**  
> Built with the sleek, clean aesthetic of modern cooling ecosystems like the **Llano V12 Ultra**, **NZXT CAM**, and **Myth Cool**.

---

## 📖 Overview

**ZXC CAM** is an open-source, ultra-low-overhead hardware monitoring and thermal management interface designed for high-performance gaming rigs, overclocked setups, and laptop cooling pad setups.

Most hardware suites on the market are bloated with telemetry services, unnecessary background processes, and forced account logins that steal precious CPU cycles. **ZXC CAM** cuts all the excess weight: offering a razor-sharp dashboard with near-zero idle utilization, instant sensor polling, and comprehensive control over your system's critical metrics.

---

## ✨ Key Features

### 🌡️ Real-Time Thermal & Workload Rings
- **CPU Telemetry:** Live package temperature, per-core load, clock frequency, wattage draw, and voltage.
- **GPU Telemetry:** Core temp, VRAM junction temp, hotspot thermals, clock speeds, and fan RPM.
- **System Memory:** RAM allocation, memory bus utilization, and available overhead.
- **Storage Metrics:** NVMe/SATA read-write activity, drive thermals, and overall disk health.

### 💨 Intelligent Fan & Cooling Curve Control
- Custom PWM fan curve profiling inspired by high-end cooling software (like **Llano V12 Ultra** and **Myth Cool**).
- Dynamic hysteresis to prevent annoying fan speed oscillations during short workload spikes.
- Preset profiles: **Silent**, **Performance**, **Extreme Gaming**, and **Custom Curve**.

### 🎨 Minimalist, Modern HUD
- Cyber-industrial, cyberpunk-inspired dark mode UI.
- Low-profile overlay mode to keep an eye on temperatures while gaming or stress-testing without FPS drops.
- RGB peripheral synchronization & lighting telemetry options.

### ⚡ True Zero-Bloat Architecture
- No mandatory accounts, login screens, or cloud DRM.
- Negligible background memory footprint (~15–30 MB RAM).
- Ring-0 hardware sensor access via low-overhead WMI and kernel sensor querying.

---

## 🖥️ System Requirements

| Component | Minimum Specification | Recommended Specification |
| :--- | :--- | :--- |
| **Operating System** | Windows 10 (64-bit) Build 19041+ | Windows 11 (64-bit) |
| **Processor** | Intel Core i3 / AMD Ryzen 3 | Intel Core i5/i7/i9 or AMD Ryzen 5/7/9 |
| **Graphics** | DirectX 11 compatible GPU | NVIDIA RTX 20/30/40/50 Series or AMD Radeon RX 6000/7000+ |
| **Permissions** | Administrator Privileges (for Ring-0 WMI & thermal diode access) | Administrator Privileges |

---

## 📥 Installation & Setup

### Method 1: Using the Installer (`.exe`)
1. Download `ZXC-Cam-Setup.exe` from the repository or the **Releases** tab.
2. Run the installer as **Administrator** (required to register Windows thermal diode providers).
3. Follow the on-screen prompts and launch **ZXC CAM**.

### Method 2: Running from Source / Desktop Shell
If you are developing or running the unpacked desktop build:
```bash
# 1. Clone the repository
git clone [https://github.com/Zachyb0i/zxc-cam.git](https://github.com/Zachyb0i/zxc-cam.git)

# 2. Navigate to the desktop bundle
cd zxc-cam/desktop

# 3. Fetch runtime dependencies and run
neu update
neu run
