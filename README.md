# NLP-Selenium-Web-Scraping
Automated web scraper to extract venture capital investor data from kando.tech including name, country, profile, and deals — exported to CSV. Built with Python and Selenium.

## 📬 Contact
Author: Amrita Veshin  
Email: amritav99@gmail.com

## Kando Investor Web Scraper - Introduction

This project scrapes investor data from [kando.tech/investors](https://kando.tech/investors/all) using Selenium and saves it to a CSV file. It extracts key fields including:

- Investor Name
- Country
- Profile Description
- Number of Deals
- Direct Profile Link

## 📦 Features

- Automated web scraping of all paginated investor listings (12,000+ entries)
- Data cleaning and structured CSV export
- Pagination support and error handling
- Chrome headless mode for efficient execution

## 🛠️ Technologies Used
- Selenium – browser automation
- Pandas – data manipulation
- tqdm – progress bar
- Google Colab – optional execution environment

## 📁 Project Contents

kando-investor-data-scraper/
│
├── Kando_Investors_WebScraping.ipynb # 💻 Main scraping notebook (Jupyter Notebook)
├── AmritaVeshin_kando_all_investors.csv # 📄 Final scraped investor dataset (12,000+ rows)
└── README.md # 📘 Documentation

## 🚀 Getting Started

### Prerequisites

- Python 3.8+
- Google Chrome
- ChromeDriver (compatible with your Chrome version)
- [Google Colab](https://colab.research.google.com/) (or local Jupyter environment)

### ✅ Setup Instructions (Google Colab Friendly)
```
# Install Chrome and dependencies
!wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb
!dpkg -i google-chrome-stable_current_amd64.deb
!apt-get -f install -y

# Check installed Chrome version
!google-chrome --version

# Install matching ChromeDriver (version 137.0.7151.68)
!wget -O /tmp/chromedriver.zip https://edgedl.me.gvt1.com/edgedl/chrome/chrome-for-testing/137.0.7151.68/linux64/chromedriver-linux64.zip
!unzip /tmp/chromedriver.zip -d /usr/bin/
!mv /usr/bin/chromedriver-linux64/chromedriver /usr/bin/chromedriver
!chmod +x /usr/bin/chromedriver
```

### Python Packages

Install dependencies:

```bash
pip install selenium pandas tqdm
```

## 🧾 Sample Output
| Name                          | Country       | Profile                        | Deals | Link                                                                                                                 |
| ----------------------------- | ------------- | ------------------------------ | ----- | -------------------------------------------------------------------------------------------------------------------- |
| New Enterprise Associates Inc | United States | Global venture capital firm... | 706   | [https://kando.tech/company/new-enterprise-associates-inc](https://kando.tech/company/new-enterprise-associates-inc) |
