# Step 5: Install Ollama (Windows and macOS)

## Goal
Install Ollama, verify the CLI works, and run your first local model.


## A. Install on Windows 10/11
1. Open https://ollama.com and download the Windows installer (`.exe`).
2. Run the installer and complete setup.
3. Open PowerShell and verify:
   ```powershell
   ollama --version
   ```
4. Run a first model:
   ```powershell
   ollama run llama3.2
   ```

## B. Install on macOS (Intel and Apple Silicon)
1. Open https://ollama.com and download the macOS installer (`.dmg`).
2. Drag **Ollama** into **Applications**.
3. Launch Ollama once so background services start.
4. Open Terminal and verify:
   ```bash
   ollama --version
   ```
5. Run a first model:
   ```bash
   ollama run llama3.2
   ```

## C. Basic Operations
- List downloaded models:
  ```bash
  ollama list
  ```
- Remove a model:
  ```bash
  ollama rm llama3.2
  ```

## D. Uninstall
### Windows
- Remove from **Settings -> Apps -> Installed apps**.
- Optionally delete `%HOMEPATH%\\.ollama` to free model storage.

### macOS
- Delete Ollama from **Applications**.
- Optionally remove `~/.ollama`.

## Troubleshooting
- `ollama` not found: restart terminal after installation.
- Download/model pull fails: confirm network access and retry.
- Slow generation: use a smaller model variant and close heavy apps.
