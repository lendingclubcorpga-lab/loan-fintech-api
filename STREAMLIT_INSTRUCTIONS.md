# Streamlit Configuration Instructions

Because I am an AI, I cannot directly click buttons, create branches, or commit code into your personal GitHub repository. You must make these modifications yourself on your **main** branch.

### Step 1: Update your configuration file
Replace your entire `pyproject.toml` file with the updated `pyproject.toml` file generated for you. This version:
1. Restricts Python to compatible versions (`>=3.9,<3.13`).
2. Forces a safe version of `pyyaml` (`>=6.0.1`).
3. Explicitly includes `streamlit` as a core dependency.

### Step 2: Clean the lock file
Delete `poetry.lock` directly from the main branch on GitHub so the server doesn't use old cache layers.

### Step 3: Change your Streamlit Cloud Deployment settings
1. Go to your Streamlit dashboard.
2. Click the three dots next to your app -> **Settings**.
3. Change the **Main file path** from `api/__init__.py` to your Streamlit user interface file (e.g., `app.py`).
