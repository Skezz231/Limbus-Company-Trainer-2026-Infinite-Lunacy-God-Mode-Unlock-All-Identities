# Git Setup Instructions

## Initial Setup (First Time)

### 1. Initialize Git Repository
```bash
git init
```

### 2. Add Remote Repository
```bash
git remote add origin https://github.com/yourusername/limbus-company-trainer.git
```

### 3. Add All Files
```bash
git add .
```

### 4. Make First Commit
```bash
git commit -m "Initial commit: Limbus Company Trainer with ImGui"
```

### 5. Push to GitHub
```bash
git branch -M main
git push -u origin main
```

## Important Notes

### Before Pushing

Make sure you have:
- ✅ Cloned ImGui into the project folder
- ✅ Built the project successfully
- ✅ Reviewed all files to ensure no sensitive data

### Files That Will NOT Be Uploaded (in .gitignore)

- `build/` - Build artifacts
- `*.exe`, `*.dll`, `*.so` - Compiled binaries
- `.vs/`, `.vscode/` - IDE settings
- `*.vcxproj`, `*.sln` - Visual Studio project files (auto-generated)
- `imgui.ini` - ImGui settings file

### Files That WILL Be Uploaded

- `src/main.cpp` - Your source code
- `CMakeLists.txt` - Build configuration
- `README.md` - Documentation
- `LICENSE` - License file
- `.gitignore`, `.gitattributes` - Git configuration
- `CONTRIBUTING.md`, `QUICKSTART.md` - Guides

### ImGui Handling

ImGui is **NOT included** in the repository. Users need to clone it:
```bash
git clone https://github.com/ocornut/imgui.git
```

This is because:
- ImGui is a third-party library
- Keeps repository size small
- Users get the latest ImGui version

## Updating Repository

### After Making Changes
```bash
git add .
git commit -m "Description of changes"
git push
```

### Creating a Release

1. Tag your version:
```bash
git tag -a v1.0.0 -m "First release"
git push origin v1.0.0
```

2. On GitHub, go to "Releases" → "Create a new release"
3. Upload your compiled `.exe` as a release asset

## Repository Structure

```
limbus-company-trainer/
├── src/
│   └── main.cpp              # Source code (TRACKED)
├── build/                     # Build directory (IGNORED)
├── imgui/                     # ImGui library (IGNORED - users clone it)
├── CMakeLists.txt            # CMake config (TRACKED)
├── README.md                 # Documentation (TRACKED)
├── LICENSE                   # License (TRACKED)
├── CONTRIBUTING.md           # Contribution guide (TRACKED)
├── QUICKSTART.md            # Quick start guide (TRACKED)
├── .gitignore               # Git ignore rules (TRACKED)
└── .gitattributes           # Git attributes (TRACKED)
```

## Common Git Commands

```bash
# Check status
git status

# See changes
git diff

# View commit history
git log --oneline

# Create new branch
git checkout -b feature-name

# Switch branches
git checkout main

# Pull latest changes
git pull

# Clone your repository
git clone https://github.com/yourusername/limbus-company-trainer.git
```

## GitHub Repository Settings

### Recommended Settings

1. **Add Topics:**
   - cpp
   - imgui
   - opengl
   - glfw
   - game-trainer
   - cmake

2. **Add Description:**
   "Educational game trainer with ImGui interface for Limbus Company"

3. **Add Website:**
   Your project website or demo (if any)

4. **Enable Issues:**
   For bug reports and feature requests

5. **Add README badges:**
   Already included in README.md

### Creating Repository on GitHub

1. Go to github.com
2. Click "+" → "New repository"
3. Name: `limbus-company-trainer`
4. Description: "Educational game trainer with ImGui interface"
5. Public/Private: Your choice
6. **Don't initialize** with README (we already have one)
7. Click "Create repository"
8. Follow the "push an existing repository" commands shown

## After Pushing

Share your repository link with:
- Build instructions in README.md
- Screenshots (add to `screenshots/` folder)
- Clear disclaimer about educational use

---

**Ready to push!** 🚀

Follow the "Initial Setup" steps above to upload your project to GitHub.
