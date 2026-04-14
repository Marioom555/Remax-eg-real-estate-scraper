# 🏡 ReMax Egypt Real Estate Scraper

A high-performance Python web scraper designed to extract real estate listings from ReMax Egypt.

It collects structured property data such as price, location, bedrooms, bathrooms, area, and more, then exports it into CSV format.

---

## 🚀 Features

- 🔁 Automatic pagination crawling
- ⚡ Multi-threaded scraping (ThreadPoolExecutor)
- 🧠 Smart retry system for failed requests
- 📍 Location parsing (City / Location1 / Location2)
- 💰 Price extraction and normalization
- 📊 Auto-saving progress every N records
- 🧹 Clean and structured data output (CSV)

---
  
## ⚙️ Installation

### 1️⃣ Clone the repository

```bash
git clone https://github.com/your-username/remax-eg-real-estate-scraper.git
cd remax-eg-real-estate-scraper
```


##  2️⃣ Install dependencies

pip install -r requirements.txt


##▶️ How to Run

python scraper/main.py


## 🛠 Tech Stack
Python 🐍
Requests
BeautifulSoup (bs4)
Pandas
Threading (concurrent.futures)


## 📈 Future Improvements
Proxy rotation support
Selenium fallback for blocked pages
Database support (SQLite / PostgreSQL)
API version (FastAPI)
Docker containerization
