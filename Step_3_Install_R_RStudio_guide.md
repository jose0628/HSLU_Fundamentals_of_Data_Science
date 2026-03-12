# Step 3: Install R and RStudio (Windows and macOS)

## Goal
Install R first, then RStudio Desktop, and verify both are working.

## Official Links (validated on 2026-03-12)
- CRAN (R downloads): https://cran.r-project.org/
- Posit RStudio Desktop downloads: https://posit.co/download/rstudio-desktop/

## A. Install R

### macOS
1. Open https://cran.r-project.org/
2. Select **Download R for macOS**.
3. Download the latest `.pkg` file for your Mac architecture.
4. Open the installer and complete the setup.
5. Verify in Terminal:
   ```bash
   R --version
   ```

### Windows
1. Open https://cran.r-project.org/
2. Select **Download R for Windows**.
3. Open **base** and download the latest installer (`.exe`).
4. Run the installer and keep default options unless instructed otherwise.
5. Verify in Command Prompt or PowerShell:
   ```powershell
   R --version
   ```

## B. Install RStudio Desktop

### macOS
1. Open https://posit.co/download/rstudio-desktop/
2. Download the macOS installer (`.dmg`).
3. Open the `.dmg` and drag **RStudio** to **Applications**.
4. Start RStudio from **Applications**.

### Windows
1. Open https://posit.co/download/rstudio-desktop/
2. Download the Windows installer (`.exe`).
3. Run installer and complete setup.
4. Start RStudio from Start Menu.

## C. Verify in RStudio
1. Open RStudio.
2. Run the following in the Console:
   ```r
   version
   print("R and RStudio are ready")
   ```
3. Confirm no startup errors.

## D. Install Core Package (optional but recommended)
In the RStudio Console, run:
```r
install.packages("tidyverse")
```

## Troubleshooting
- R not detected by RStudio: reinstall R first, then restart RStudio.
- macOS security warning: right-click installer and choose **Open**.
- Windows permission issues: run installer as administrator.
- Package installation errors: choose a CRAN mirror and retry.
