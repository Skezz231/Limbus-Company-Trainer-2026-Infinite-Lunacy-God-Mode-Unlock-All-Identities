# Quick Start Guide

## For Windows Users

### Prerequisites
- Visual Studio 2019+ (with C++ development tools)
- CMake 3.10+
- Git

### Build Steps

1. Open PowerShell or CMD in your project folder

2. Clone ImGui:
```powershell
git clone https://github.com/ocornut/imgui.git
```

3. Build the project:
```powershell
mkdir build
cd build
cmake ..
cmake --build . --config Release
```

4. Run:
```powershell
.\Release\LimbusCompanyTrainer.exe
```

## For Linux Users

### Prerequisites
```bash
sudo apt-get install build-essential cmake libglfw3-dev libgl1-mesa-dev git
```

### Build Steps
```bash
git clone https://github.com/ocornut/imgui.git
mkdir build && cd build
cmake ..
make
./LimbusCompanyTrainer
```

## For macOS Users

### Prerequisites
```bash
brew install cmake glfw
```

### Build Steps
```bash
git clone https://github.com/ocornut/imgui.git
mkdir build && cd build
cmake ..
make
./LimbusCompanyTrainer
```

## Troubleshooting

### Issue: CMake can't find GLFW
**Solution:** Make sure GLFW is properly installed or let CMake download it automatically (already configured in CMakeLists.txt)

### Issue: ImGui folder not found
**Solution:** Clone ImGui into the project root:
```bash
git clone https://github.com/ocornut/imgui.git
```

### Issue: Build fails on Windows
**Solution:** 
- Ensure Visual Studio C++ tools are installed
- Try running CMake from "Developer Command Prompt for VS"

### Issue: Missing OpenGL
**Solution:**
- **Windows:** Usually included with graphics drivers
- **Linux:** `sudo apt-get install libgl1-mesa-dev`
- **macOS:** Included with Xcode Command Line Tools

## Features Overview

After launching, you'll see:
- **Left Panel:** Game statistics (updates in real-time)
- **Center:** Cheat menu with tabs (Resources, Combat, Automation, Misc, Info)
- **Bottom:** Notifications panel

### How It Works
1. Wait 3 seconds for "game connection" (simulation)
2. All features unlock after connection
3. Toggle cheats and see stats update
4. Notifications appear for each action

## Need Help?

Open an issue on GitHub with:
- Your OS and version
- CMake version
- Error messages (if any)
- Steps you've tried

---

Happy coding! ⭐
