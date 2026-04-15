# 🧪 Benchmark

> **PowerShell System Performance Benchmark Suite** - Comprehensive CPU, Memory, Disk, GPU, and Network testing tool.

---

## 📋 Overview

Benchmark is a comprehensive system performance testing suite written in PowerShell. It provides detailed performance metrics across all major system components with calibrated scoring for easy comparison.

### 🎯 What It Does

- 🖥️ **CPU Benchmarking** - Prime calculation and mathematical operations
- 🧠 **Memory Testing** - Array operations and random access patterns
- 💾 **Disk I/O Testing** - Read/write speed analysis
- 🎮 **GPU Compute Testing** - Matrix multiplication and trigonometric operations
- 🌐 **Network Testing** - Latency and download speed measurement
- 📊 **Scored Results** - Calibrated percentage-based performance ratings

---

## 📁 Project Structure

| File | Description |
|------|-------------|
| `Benchmark.exe` | Compiled C# GUI executable |
| `Benchmark.ps1` | Main PowerShell benchmark script |
| `BenchmarkEngine.cs` | C# benchmarking engine source |
| `BenchmarkResults.cs` | Results handling source code |
| `MainForm.cs` | Windows Forms GUI implementation |
| `Program.cs` | Application entry point |
| `app.manifest` | Application manifest |
| `Autorun.ico` | Application icon |
| `build.bat` | Build automation script |

---

## 🚀 Usage

### PowerShell Script

```powershell
# Run the benchmark
.\Benchmark.ps1

# Results will display in console with color-coded performance ratings
```

### Compiled Executable

```cmd
# Run the GUI version
.\Benchmark.exe
```

### Build from Source

```cmd
# Build the C# project
.\build.bat
```

---

## 📊 Benchmark Tests

### 🖥️ CPU Test
- **Method**: Prime calculation (up to 50,000) + 1,000,000 math operations
- **Metrics**: Primes found, execution time, CPU score
- **Reference Score**: 75,000 points
- **Display**: Cyan (≥100%), Green (75-99%), Yellow (50-74%), Red (<50%)

### 🧠 Memory Test
- **Method**: 10 million element array operations
  - Write test: Populate ArrayList
  - Read test: Sum all elements
  - Random access: 100,000 random lookups
- **Metrics**: Total RAM, execution time, memory score
- **Reference Score**: 4,600 points

### 💾 Disk I/O Test
- **Method**: 100 MB sequential read/write
- **Metrics**: Write MB/s, Read MB/s, average disk score
- **Reference Score**: 4,600 points

### 🎮 GPU Test
- **Method**: 200x200 matrix multiplication + 100,000 trig operations
- **Metrics**: GPU name, VRAM, execution time, GPU score
- **Reference Score**: 1,000 points

### 🌐 Network Test
- **Method**:
  - Latency: Ping to 8.8.8.8, 1.1.1.1, and google.com
  - Download: 10MB test file from multiple sources
- **Metrics**: Average latency, download speed Mbps, network score
- **Reference Score**: 25 points

---

## 📈 Scoring System

All tests use calibrated reference scores based on typical modern mid-range systems:

| Component | Reference Score | Unit |
|-----------|----------------|------|
| CPU | 75,000 | Points |
| Memory | 4,600 | Points |
| Disk | 4,600 | MB/s average |
| GPU | 1,000 | Points |
| Network | 25 | Mbps + latency |

### Performance Ratings
- 🔵 **≥ 100%** - Excellent (Above mid-range)
- 🟢 **75-99%** - Good (Mid-range performance)
- 🟡 **50-74%** - Fair (Below mid-range)
- 🔴 **< 50%** - Poor (Significantly below mid-range)

---

## 🔧 Technical Details

### PowerShell Script
- **Language**: PowerShell 5.1+
- **Dependencies**: Windows Management Instrumentation (WMI)
- **Elevation**: Not required for basic tests

### C# Application
- **Framework**: .NET Framework 4.x
- **UI**: Windows Forms
- **Architecture**: x64

---

## 📋 Requirements

### Minimum
- Windows 7 SP1 or later
- PowerShell 5.1 (for script) or .NET Framework 4.5 (for executable)
- 100 MB free disk space

### Recommended
- Windows 10/11
- Multi-core CPU
- 8 GB+ RAM
- SSD for accurate disk testing

---

## 🎨 Output Example

```
========================================
  POWERSHELL SYSTEM BENCHMARK SUITE
========================================

System: Microsoft Windows 11 Pro
PowerShell: 5.1.22621.1778
Date: 2024-01-15 14:32:10

========================================
  CPU BENCHMARK
========================================

[INFO] CPU: Intel(R) Core(TM) i7-12700K
[INFO] Cores: 12 | Threads: 20
[INFO] Running prime calculation test...

[RESULT] Primes Found: 5133
[RESULT] Time: 1.25 seconds
[RESULT] CPU Score: 80000
[RESULT] CPU Performance: 106.7%

========================================
  FINAL RESULTS
========================================

Component Scores:
  CPU      : 80000 [106.7%]
  Memory   : 4800 [104.3%]
  Disk I/O : 5200 [113.0%]
  GPU      : 1100 [110.0%]
  Network  : 28 [112.0%]

========================================
  OVERALL SCORE: 83720 [109.3%]
========================================
```

---

## ⚠️ Important Notes

- 📝 Temporary files are created in `%TEMP%` during disk testing and cleaned up automatically
- 🌐 Network test requires internet connectivity
- ⏱️ Results may vary based on system load during testing
- 🔄 For consistent results, close other applications before running
- 💾 Disk test writes 100 MB - ensure sufficient free space

---

## 📜 License & Disclaimer
---

## Comprehensive legal disclaimer

This project is intended for authorized defensive, administrative, research, or educational use only.

- Use only on systems, networks, and environments where you have explicit permission.
- Misuse may violate law, contracts, policy, or acceptable-use terms.
- Running security, hardening, monitoring, or response tooling can impact stability and may disrupt legitimate software.
- Validate all changes in a test environment before production use.
- This project is provided "AS IS", without warranties of any kind, including merchantability, fitness for a particular purpose, and non-infringement.
- Authors and contributors are not liable for direct or indirect damages, data loss, downtime, business interruption, legal exposure, or compliance impact.
- You are solely responsible for lawful operation, configuration choices, and compliance obligations in your jurisdiction.

---

<p align="center">
  <sub>Built with care by <strong>Gorstak</strong></sub>
</p>