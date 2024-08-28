---
title: "Installing Python"
published: true
morea_id: reading-python-install
morea_summary: "Installing and using Python"
morea_type: reading
morea_sort_order: 4
morea_start_date: 
  "Section 1": "2024-08-29T10:30"
  "Section 2": "2024-08-30T12:00"
---
# Installing Python from Python.org

## Step 1: Download Python

1. **Visit the Official Python Website**:
   - Go to the [official Python website](https://www.python.org/).

2. **Navigate to the Downloads Section**:
   - On the homepage, you'll see a prominent "Downloads" button.
   - The website automatically detects your operating system and suggests the latest version of Python. 
   - Click the "Download Python X.Y.Z" button (where X.Y.Z is the latest version number).

3. **Choose Your Operating System** (if needed):
   - If you're downloading for a different operating system, click the "View the full list of downloads" link on the Downloads page.
   - Select the appropriate installer for your operating system:
     - **Windows**: Download the executable installer (`.exe`).
     - **macOS**: Download the installer package (`.pkg`).
     - **Linux/Unix**: Download the source code or use the package manager of your distribution.

## Step 2: Install Python

### Windows

1. **Run the Installer**:
   - Locate the downloaded `.exe` file in your `Downloads` folder and double-click to run it.

2. **Customize Installation (Optional)**:
   - The installer provides options to customize the installation.
   - Ensure that you check the box that says **"Add Python to PATH"** at the bottom of the window. This is important for running Python from the command line.

3. **Install Python**:
   - Click "Install Now" to begin the installation with default settings, or choose "Customize installation" to select specific features.
   - Wait for the installation to complete, then click "Close."

### macOS

1. **Run the Installer**:
   - Open the downloaded `.pkg` file to start the installation.

2. **Install Python**:
   - Follow the on-screen instructions to install Python.
   - The installer will place Python in `/usr/local/bin` and the "Python Launcher" in `/Applications`.

3. **Verify Installation**:
   - Open a terminal and run the following command to verify the installation:
     ```bash
     python3 --version
     ```
   - You should see the Python version installed.

### Linux/Unix

1. **Install via Package Manager**:
   - Most Linux distributions include Python by default. However, if you need to install or upgrade Python, use your distribution’s package manager.
   - For example, on Ubuntu:
     ```bash
     sudo apt update
     sudo apt install python3
     ```

2. **Verify Installation**:
   - Open a terminal and run:
     ```bash
     python3 --version
     ```
   - You should see the installed Python version.

## Step 3: Verify Python Installation

1. **Open a Command Line Interface**:
   - On **Windows**, open `Command Prompt` or `PowerShell`.
   - On **macOS** or **Linux**, open the `Terminal`.

2. **Check Python Version**:
   - Run the following command to verify the installation:
     ```bash
     python --version
     ```
   - On some systems, you might need to use `python3` instead:
     ```bash
     python3 --version
     ```

   - You should see the Python version number displayed, confirming that Python is installed correctly.

## Step 4: Install pip

- **pip** is the package installer for Python, included by default with Python 3.4+.
- Verify pip installation by running:
  
  ```bash
  pip --version
  ```