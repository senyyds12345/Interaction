# Interaction - Termux Multi-Language Interactive Runner

A Bash script tailored for Termux, supporting interactive execution of **Java, Python, C++, PHP, and JavaScript**. It automatically checks and installs missing dependencies, designed for both beginners and developers.


## 🚀 Core Features
- 🔍 **Auto-Dependency Check**: Verifies installations of OpenJDK (Java), Python3, g++ (C++), Node.js, and PHP on launch; prompts to install missing packages.
- 🖥️ **One-Click Mode Switch**: Defaults to Java Mode. Switch via keywords: `cpp` (C++), `python`, `php`, `js` (JavaScript).
- 📱 **Termux-Native**: No root required, optimized for mobile terminals with minimal storage usage.
- 🧹 **Auto-Cleanup**: Deletes C++ compilation artifact (`main` binary) after execution to avoid clutter.


## 📦 Installation (Termux Exclusive)
### Method 1: Install via DEB Package (Recommended)
1. Download the DEB package from the repository:  
   [interaction-termux_1.0-1_all.deb](https://github.com/your-username/your-repo/blob/main/interaction-termux_1.0-1_all.deb)  
   (Replace the link with your actual GitHub DEB package URL)

2. Navigate to the download directory in Termux:
   ```bash
   # Example: If downloaded to Termux's "Downloads" folder
   cd ~/Downloads
