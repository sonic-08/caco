# Caco Calculator

Caco is a calculator app for Linux featuring graph plotting, theme support, and a minimal interface.



## Prerequisites

Before setting up Caco, ensure you have **Node.js** and **npm** installed on your Linux distribution.

## Install Node.js & npm

### Ubuntu / Debian

```bash
sudo apt update
sudo apt install nodejs npm
```

### Fedora

```bash
sudo dnf install nodejs npm
```

### Arch Linux

```bash
sudo pacman -S nodejs npm
```

---

# Setup Instructions

## 1. Navigate to the Project Directory

Open your terminal and move into the folder where you extracted or cloned the Caco source code.

```bash
cd ~/caco
```

---

## 2. Install Dependencies

This installs the internal JavaScript logic, styling engines, and the Electron builder.

```bash
npm install
```

---

## 3. Build the Application

This compiles the source code and packages it into a native Linux binary.

```bash
npm run package
```

---

# Installation

To install the build locally so it launches like a normal desktop application:

```bash
# Remove any existing installation
rm -rf ~/.local/share/caco

# Move the newly built binary into your local share directory
mv out/*-linux-x64 ~/.local/share/caco
```

---

# How to Update

Whenever you make changes to the code:

```bash
cd ~/caco

rm -rf out/

npm run package

rm -rf ~/.local/share/caco

mv out/*-linux-x64 ~/.local/share/caco
```

---

# Launching

Launch directly from the terminal:

```bash
~/.local/share/caco/caco
```

Or simply search for **"Caco"** in your GNOME or KDE application menu.

---

# Features

* Glassmorphism-inspired UI
* Interactive graph plotter
* Dynamic theme support
* Native Linux packaging
* Minimalist interface
* Electron-powered desktop app

---

# Tech Stack

* Electron
* Node.js
* npm
* JavaScript

---

# License

MIT License
