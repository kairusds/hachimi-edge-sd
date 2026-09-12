# hachimi-edge-sd

Bare translations for Hachimi Edge to use for its "Skill data descriptions" feature.

## How to use

1. Install Python 3.11 or newer: https://www.python.org/downloads/
2. Create a virtual environment: `python -m venv .venv`
3. Activate it:
  - Linux: `source .venv/bin/activate`
  - Windows (cmd): `.venv\Scripts\activate.bat`
  - Windows (PowerShell): `.venv\Scripts\Activate.ps1`
    - If blocked by execution policy:
      `powershell -ExecutionPolicy Bypass -File .venv\Scripts\Activate.ps1`
    - Or permanently:
      `Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy RemoteSigned`
4. Install dependencies: `pip install -r requirements.txt`
5. Ensure there's at least one commit: `git rev-parse HEAD || (git add -A && git commit -m "Init")`
6. Regenerate `index.json` whenever you change the files under `localized_data/`: `python gen_index.py`
 - Run `deactivate` to leave the environment once you're done.
