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

---

## The Digital Guestbook

This project also includes `The Digital Guestbook.ipynb`, a Jupyter Notebook that demonstrates how to interact with a Google Sheet to create a digital guestbook.

### How to Use the Notebook

1.  **Open the Notebook:**
    *   Open `The Digital Guestbook.ipynb` in a Jupyter environment (like Jupyter Lab or Visual Studio Code).

2.  **Follow the Instructions:**
    *   The notebook contains detailed instructions in the first markdown cell. Follow these instructions to:
        *   Set up a Google Cloud Project.
        *   Enable the required APIs.
        *   Create a service account and download the JSON key.
        *   Create a Google Sheet and share it with the service account.

3.  **Run the Cells:**
    *   Run the cells in the notebook in order. The notebook will guide you through installing the necessary libraries and running the guestbook application.