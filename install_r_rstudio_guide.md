---
title: "Installing R and RStudio on macOS and Windows"
date: "2025-02-19"
---

# Installing R and RStudio on macOS and Windows

A quick guide to help you install **R** (the programming language) and **RStudio** (the IDE) on both macOS and Windows. Typically, install **R** first, then **RStudio**.

---

## Table of Contents

1. [Prerequisites](#prerequisites)  
2. [Installing R](#installing-r)  
   - [macOS](#macos)  
   - [Windows](#windows)  
3. [Installing RStudio](#installing-rstudio)  
   - [macOS](#macos-1)  
   - [Windows](#windows-1)  
4. [Verifying Your Installation](#verifying-your-installation)  
5. [Installing Packages](#installing-packages)  
6. [Keeping R and RStudio Updated](#keeping-r-and-rstudio-updated)  
7. [Troubleshooting](#troubleshooting)  

---

## Prerequisites

- **Administrator access** on your computer (you may need to enter a password to confirm installations).  
- **Internet connection** for downloading R, RStudio, and packages.  

---

## Installing R

### macOS

1. **Go to the [CRAN website](https://cran.r-project.org/).**  
2. Click **Download R for (Mac) OS X**.  
3. Under **Latest release**, download the `.pkg` file for the latest R version.  
4. Open the `.pkg` file (usually located in your **Downloads** folder).  
5. Follow the on-screen installation prompts (enter your password if prompted).  

**Tip**: After installation, verify R by opening **Terminal** and typing:
```bash
R --version
```
You should see information about your R version.

### Windows

1. **Go to the [CRAN website](https://cran.r-project.org/).**  
2. Click **Download R for Windows**.  
3. Choose **base** and download the `.exe` installer for the latest version of R.  
4. Locate the installer (usually in your **Downloads** folder) and double-click it.  
5. Follow the prompts in the R Setup Wizard (accepting defaults is typically fine).  

**Tip**: After installation, verify R by opening **Command Prompt** and typing:
```bash
R --version
```
You should see your installed R version displayed.

---

## Installing RStudio

### macOS

1. **Go to the [Posit RStudio download page](https://posit.co/download/rstudio-desktop/).**  
2. Under **All installers**, find the macOS installer (e.g., `RStudio-202X.X.X.dmg`).  
3. Double-click the downloaded `.dmg` file.  
4. In the window that appears, drag the **RStudio** icon into the **Applications** folder.  
5. Launch **RStudio** from the **Applications** folder or from **Launchpad**.

### Windows

1. **Go to the [Posit RStudio download page](https://posit.co/download/rstudio-desktop/).**  
2. Download the **Windows** installer (e.g., `RStudio-202X.X.X.exe`).  
3. Double-click the installer to begin setup.  
4. Follow the installation prompts (defaults are typically fine).  
5. Launch **RStudio** from the **Start menu** or from any shortcut you created.

---

## Verifying Your Installation

1. **Open RStudio**:  
   - On macOS, find it in **Applications** or **Launchpad**.  
   - On Windows, find it in the **Start menu** or your **Desktop**.  

2. **Check R Version**: RStudio should auto-detect your R installation.  
   - In RStudio, go to **Tools > Global Options** (on macOS, **RStudio > Preferences...**).  
   - Under **General**, you’ll see the path to R that RStudio is using.  

3. **Run a Test Command**: Type into the **Console** in RStudio:
   ```r
   print("Hello, RStudio!")
   ```
   Press **Enter** (or **Return**). You should see `[1] "Hello, RStudio!"` in the Console output.

---

## Installing Packages

R comes with base packages, but you might want more. For example, install the **tidyverse** (includes `dplyr`, `ggplot2`, etc.) with:

```r
install.packages("tidyverse")
```

You can also install other packages by using:

```r
install.packages("<package-name>")
```

---

## Keeping R and RStudio Updated

- **Update R**: Periodically check [CRAN](https://cran.r-project.org/) for new R releases.  
- **Update RStudio**: In RStudio, go to **Help > Check for Updates** or visit the [RStudio download page](https://posit.co/download/rstudio-desktop/) for the newest version.

---

## Troubleshooting

- **macOS Permissions**: If you encounter a permission issue, right-click the `.pkg` or `.dmg` file and choose **Open**. You may also need to allow apps from “identified developers” in **System Settings > Privacy & Security**.  
- **Windows Antivirus**: Some antivirus software may flag or slow installation. Temporarily disable it if you trust the source.  
- **Multiple R Versions**: If you have multiple R versions installed, specify which version RStudio should use in **Tools > Global Options > General > R Version**.  
- **R Not Detected**: If RStudio doesn’t detect R, reinstall R, then restart RStudio, or manually point RStudio to the correct R installation path.

---

**Congratulations!** You have successfully installed R and RStudio. You’re now ready to begin data analysis, statistical computing, and data visualization with R. Enjoy!
