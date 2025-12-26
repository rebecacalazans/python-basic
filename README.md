# Music Explorer Project

This project uses the Spotify API to explore artists and their top tracks.

## Setup

To use this project, you need to provide your Spotify API credentials. You can do this by creating a `config.py` file in the root of the project.

### Create the `config.py` file

Create a file named `config.py` in the main directory of this project with the following content:

```python
# Spotify API Credentials
CLIENT_ID = "YOUR_CLIENT_ID"
CLIENT_SECRET = "YOUR_CLIENT_SECRET"
REDIRECT_URI = "http://127.0.0.1:8888/callback"
```

**Important:**
*   Replace `"YOUR_CLIENT_ID"` and `"YOUR_CLIENT_SECRET"` with your actual Spotify API credentials.
*   Make sure the `REDIRECT_URI` matches the one you have configured in your Spotify Developer Dashboard.
*   **Do not share your `config.py` file or commit it to version control.** It contains sensitive information. The `.gitignore` file is already configured to ignore this file.

### Spotify Developer Dashboard

Ensure that the `REDIRECT_URI` in your `config.py` file is also added to the "Redirect URIs" list in your Spotify Developer Dashboard under your application's settings.
