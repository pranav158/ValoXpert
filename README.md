# ValoXpert

ValoXpert is a Windows optimization tool designed to enhance gaming performance for Valorant.

## Features

### 🔧 Service Management
- Automatically detects and manages non-essential Windows services.
- Smart service detection to avoid disabling critical system services.
- Caches service states for quick restoration.
- Dependency-aware service management to ensure stability.

### 🚀 Performance Optimization
- CPU core optimization for both Intel and AMD processors.
- Game process priority and affinity management.
- Memory optimization for better gaming performance.
- Custom desktop mode to reduce background distractions during gaming sessions.

### 🖥 CPU Optimization
- **Detects CPU architecture (Intel/AMD) and their specific features.**

#### For Intel:
- Identifies P-cores and E-cores in hybrid architectures.
- Prioritizes P-cores for gaming.
- Uses E-cores only when necessary.
- Optimizes thread distribution based on core type.

#### For AMD:
- Identifies CCX (Core Complex) groupings.
- Optimizes core allocation within the same CCX to minimize latency.
- Balances thread distribution across available cores.

### ⚡ Advanced Features
- NUMA node awareness.
- Thread-level optimization.
- Intelligent core distribution.
- Fallback mechanisms for unsupported configurations.

### 🔐 Safety Features
- Automatic detection of system-critical services.
- Service state backup before making changes.
- Fail-safe restoration process.
- Dynamic adjustment based on available resources.

### 🛠 Memory Management
- Uses direct Windows API calls to clear the standby list.
- Attempts multiple memory purge operations for better effectiveness.
- Properly handles privileges needed for memory operations.

### 🎨 User Interface
- Clean and modern UI built using Siticone Desktop UI.
- Real-time service status monitoring.
- Detailed logging system for troubleshooting.
- Easy-to-use toggle switches for enabling/disabling features.

### ⚙️ Configuration
- Automatic service state backup and restoration.
- Custom service management via the Settings panel.

## 🛠 Usage
1. Launch **ValoXpert**.
2. Select desired optimizations in the **Settings** panel.
3. Apply changes.
4. Launch your game.
5. Once finished, close the game and it will automatically revert system settings to normal.

## 🖥 System Requirements
- Windows 10/11
- .NET Framework 4.8

## 🤝 Contributing
Contributions are welcome! Please read through the code documentation and follow the existing coding style when submitting pull requests.

## 📜 License
**All rights reserved.** This project is proprietary software and not open-source.

---

### 📌 Notes
- **Settings are stored in:** `...` *AppData\Local\Mystic\services.cache*
- **Service states are cached in:** `...` *AppData\Local\Mystic\ValoXpert.conf*
