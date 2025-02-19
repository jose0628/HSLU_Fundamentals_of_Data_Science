# Installing Git on macOS and Windows

## Installing Git on macOS

### Method 1: Install Git Using Xcode Command Line Tools (Recommended)
1. Open **Terminal** (`Command + Space`, then type **Terminal** and hit **Enter**).
2. Run the following command:
   ```sh
   git --version
   ```
3. If Git is not installed, you will see a prompt to install it. Click **Install** and follow the instructions.
4. After installation, verify with:
   ```sh
   git --version
   ```

### Method 2: Install Git via Homebrew
1. Install Homebrew (if not already installed):
   ```sh
   /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
   ```
2. Install Git:
   ```sh
   brew install git
   ```
3. Verify installation:
   ```sh
   git --version
   ```

### Method 3: Download Git Installer
1. Visit [Git's official website](https://git-scm.com/downloads).
2. Download the macOS `.dmg` installer.
3. Open the installer and follow the installation steps.
4. Verify the installation:
   ```sh
   git --version
   ```

## Installing Git on Windows

### Method 1: Install Git Using Git for Windows (Recommended)
1. Download **Git for Windows** from [Git for Windows](https://gitforwindows.org/).
2. Run the installer and follow these recommended settings:
   - Use Git from the Windows Command Prompt.
   - Choose a default text editor (Vim, Nano, or Notepad++).
   - Select **Checkout Windows-style, commit Unix-style line endings**.
   - Use **MinTTY (default terminal)**.
   - Complete the installation.
3. Verify the installation:
   ```sh
   git --version
   ```

### Method 2: Install Git via Winget (Windows Package Manager)
1. Open **Command Prompt** or **PowerShell** as Administrator.
2. Run:
   ```sh
   winget install --id Git.Git -e --source winget
   ```
3. Verify installation:
   ```sh
   git --version
   ```

## Setting Up Git After Installation
1. Configure Git with your name and email:
   ```sh
   git config --global user.name "Your Name"
   git config --global user.email "your-email@example.com"
   ```
2. Check your configuration:
   ```sh
   git config --list
   ```

Now Git is installed and ready to use on macOS or Windows! 🚀
