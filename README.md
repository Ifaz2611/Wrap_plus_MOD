# 🚀 WARP (1.1.1.1) Automation Script

An automation tool written in **Python** to simulate referral registrations for **Cloudflare WARP+** (1.1.1.1), boosting data balance via generated installation IDs.

> ⚠️ **Disclaimer**: This project is for educational purposes only. Misuse may violate Cloudflare’s Terms of Service.

## 📌 Features

- 🔁 Automated referral requests to WARP+ API
- 🔒 Proxy support (HTTP/S)
- ⚙️ Configurable cooldown and retry logic
- 🧪 Randomized data generation (install ID, key, token)
- 🪵 Custom logging levels for easier debugging
- 📊 Tracks successful and failed attempts

## 🛠️ Requirements

- Python 3.7+
- [httpx](https://www.python-httpx.org/)
  
Install dependencies:

```bash
pip install httpx
📂 Configuration
Modify these variables in the script to suit your environment:

python
Copy
Edit
WARP_CLIENT_ID = "your-referral-id-here"
USE_PROXY = True or False
PROXY_URL = "http://your-proxy:port"
LOG_LEVEL = "INFO"
You can also tweak:

COOLDOWN_RANGE_MIN, COOLDOWN_RANGE_MAX – how long the script waits between attempts

MAX_RETRIES – how many times a failed request is retried

▶️ Running the Script
Simply run:

bash
Copy
Edit
python warp_script.py
The script will continuously:

Generate random device data

Send requests to Cloudflare's WARP API

Log and count the success/failure rates

Sleep for a random cooldown period before repeating

📡 Proxy Support
To use a proxy:

Set USE_PROXY = True

Provide a valid PROXY_URL, e.g., "http://127.0.0.1:8080"

📝 Notes
Be aware of your legal responsibility when using automation against third-party services.

Excessive or abusive behavior might lead to your account being flagged or banned.

🧠 Credits
Inspired by various open-source WARP+ automation scripts.

Developed by Ifaz2611

🛑 Disclaimer
This script is not affiliated with or endorsed by Cloudflare. The author is not responsible for any misuse or consequences arising from the use of this tool.

