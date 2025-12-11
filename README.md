# Anomaly Detection Streamlit (Binder)

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/pedromanuelmarques-web/anomaly/main?urlpath=proxy/8501/)

This repository hosts a **Streamlit Anomaly Detection** app and Binder configuration so you can run it directly in the browser, no installs needed.

## Quick Start (Binder)
Click the badge above or use this URL:

```
https://mybinder.org/v2/gh/pedromanuelmarques-web/anomaly-detection-streamlit-binder/main?urlpath=proxy/8501/
```

> Keep the trailing slash at the end of `proxy/8501/`.

## Files
- `app.py` – Streamlit app (training + detection + interactive charts)
- `requirements.txt` – Python deps (includes `jupyter-server-proxy`)
- `runtime.txt` – Python 3.11 pin
- `.binder/start` – starts Streamlit then JupyterLab
- `.binder/postBuild` – sets executable bit + enables server proxy

## Local run
```bash
pip install -r requirements.txt
streamlit run app.py
```

## Notes
- Streamlit is bound to `0.0.0.0` and CORS disabled when proxied via Jupyter.
- If Binder is busy or the event stream fails, retry later or in an incognito window.
```
