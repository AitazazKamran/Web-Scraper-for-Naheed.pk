# Web-Scraper-for-Naheed.pk

This Python script scrapes product information (name and price) from the search results page of Naheed.pk using rotating proxies with authentication. The extracted data is saved into a CSV file.

Features

Uses BeautifulSoup for web scraping

Supports rotating proxies with authentication

Extracts product names and prices

Saves data to a CSV file

Installation

Clone this repository:

git clone https://github.com/yourusername/naheed-webscraper.git
cd naheed-webscraper

Install dependencies:

pip install -r requirements.txt

Dependencies

Ensure you have the following Python libraries installed:

pip install requests beautifulsoup4 pandas

Usage

Run the script:

python scraper.py

Configuration

Proxies

This script uses authenticated proxies for anonymous scraping. Update the proxies list in scraper.py with your working proxy credentials:

proxies = [
    {"http": "http://username:password@198.23.239.134:6540", "https": "http://username:password@198.23.239.134:6540"},
    {"http": "http://username:password@207.244.217.165:6712", "https": "http://username:password@207.244.217.165:6712"}
]

Output

The scraped data is stored in a CSV file:

product_data.csv

Each row contains:

Product Name

Product Price

Example Output

Product Name

Product Price

Basmati Rice 5kg

Rs. 1,500

Organic Brown Rice 2kg

Rs. 850

Error Handling

Timeout Handling: Requests have a timeout=10 to prevent hanging.

Request Failures: Failed requests are logged with the proxy used.

License

This project is licensed under the MIT License.

Author

Muhammad Aitazaz Kamran

⭐ If you find this project helpful, please consider giving it a star!
