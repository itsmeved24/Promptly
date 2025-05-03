Promptly
A bot that sends **fun, warm "Good Morning / Custom Prompted" messages** with images to your loved ones via WhatsApp—automatically, every day. Never forget to check in again 😉

🚀 Features
* 📸 Fetches random images from Unsplash
* 💬 Sends scheduled messages via WhatsApp
* 📝 Logs events and errors
* ⚙️ Fully customizable messages, timing, and images

🧰 Tech Stack
* **Python** – Core logic
* **Unsplash API** – Image fetching
* **PyWhatKit** – WhatsApp automation
* **Schedule** – Task scheduler

⚙️ Setup & Usage
1. Clone & Install

```bash
git clone https://github.com/itsmeved24/Promptly.git  
cd Promptly  
pip install -r requirements.txt  
```

2. Configure `.env`
Create a `.env` file in the root directory:

```
PHONE_NUMBER=+911234567890
UNSPLASH_API_KEY=your_unsplash_api_key_here
```

3. Run

```bash
python main.py
```

🔧 Customization
* **Change message text** → Edit in `main.py`
* **Use different image keywords** → Edit `image_fetcher.py`
* **Adjust time** → `schedule.every().day.at("HH:MM")` in `main.py`
* **Use personal images** → Drop them into `images/` and modify logic

🪵 Logging
Logs (`image_fetcher.log`) include:
* Fetch timestamps
* Success/failure messages
* Image URLs & query terms
* Errors & exceptions
* Debug info

📁 Structure
```
.
├── images/
├── .env
├── image_fetcher.py
├── main.py
├── image_fetcher.log
├── requirements.txt
...
```

🤝 Contribute
Pull requests are welcome!

📄 License
MIT