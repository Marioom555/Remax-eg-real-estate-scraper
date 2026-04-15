# 🏡 ReMax Egypt Real Estate Scraper (Sequential Version)

A clean and reliable Python web scraper for extracting real estate listings from ReMax Egypt.

This version runs in a **sequential mode (no threading)** for better stability and easier debugging.

---

## 🚀 Features

- 🔁 Automatic pagination crawling
- 🌐 Safe HTTP requests with retry mechanism
- 🧹 Clean text extraction and normalization
- 📍 Smart location parsing (City / Location1 / Location2)
- 💰 Price extraction and price-per-meter calculation
- 🏷️ Rent / Sale detection
- 💾 Auto-saving progress every N records
- 🧾 Final structured CSV output

---

## 📁 Project Structure
```bash
remax-eg-scraper/
│
├── scraper.py
├── remax_partial.csv
├── remax_final.csv
├── requirements.txt
└── README.md
```



---

## ⚙️ Installation

### 1️⃣ Clone the repository

```bash
git clone https://github.com/your-username/remax-eg-scraper.git
cd remax-eg-scraper
```

## 2️⃣ Install dependencies

```
pip install -r requirements.txt
```

## ▶️ How to Run

```
python scraper.py
```
## 📊 Output Files

After running the scraper, you will get:

📄 remax_final.csv

Final dataset containing all scraped properties.

## 🧠 Data Fields

The scraper extracts structured real estate data as follows:

| Description | Field |
|------|------|
| Property URL | Link |
| Number of bedrooms | Bedrooms |
| Number of bathrooms | Bathrooms |
| Property size (sqm) | Area |
| Listing price | Price |
| Calculated price per sqm | Price_per_meter |
| Full raw address | Address |
| Extracted city | City |
| Main area | Location1 |
| Sub area | Location2 |
| Rent or Sale type | Rent_sale |


## ⚙️ Configuration

```
base_url = "https://remax.com.eg"
SAVE_EVERY = 100
```

## 🛠 Tech Stack
*  Python 🐍
*  Requests
*  BeautifulSoup (bs4)
*  Pandas
*  Regular Expressions (re)

## 📈 Future Improvements
*  Proxy rotation for anti-blocking
*  Async version (faster crawling)
*  Database storage (SQLite / PostgreSQL)
*  API wrapper using FastAPI
*  Docker containerization
