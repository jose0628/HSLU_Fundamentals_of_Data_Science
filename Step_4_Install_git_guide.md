# Step 4: Install Git (Windows and macOS)

## Goal
Install Git and apply basic configuration for coursework.

## Official Links (validated on 2026-03-12)
- Git downloads: https://git-scm.com/downloads
- Git for Windows: https://gitforwindows.org/

## A. Install on macOS

### Option 1 (recommended): Xcode Command Line Tools
1. Open Terminal.
2. Run:
   ```bash
   git --version
   ```
3. If prompted, install Command Line Tools.
4. After installation, run `git --version` again.

### Option 2: Official installer
1. Open https://git-scm.com/downloads
2. Download the macOS installer.
3. Install and verify with:
   ```bash
   git --version
   ```

## B. Install on Windows
1. Open https://gitforwindows.org/
2. Download and run the installer.
3. During setup, use these defaults unless your team requires something else:
   - Git from command line and 3rd-party tools.
   - Checkout Windows-style, commit Unix-style line endings.
4. Verify in PowerShell:
   ```powershell
   git --version
   ```

## C. First-Time Git Configuration
Run these commands after installation:

```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
git config --global init.defaultBranch main
```

Verify:
```bash
git config --global --list
```

## Troubleshooting
- `git` command not found: restart terminal after install.
- Wrong username/email in commits: rerun `git config --global` commands.
- Windows path issues: open a new PowerShell window and retry.
