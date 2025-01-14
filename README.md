# Kijiji Student Housing Scraper

This project is a very basic Python-based scraper designed to collect student housing listings from Kijiji, focusing on the Kingston area. The data scraped includes listing details such as the title, price, address, number of bedrooms, number of bathrooms, and the date posted. The scraper processes a page of listings and stores the results in an Excel file.

## Features

- Scrapes listings from Kijiji within a 5 km radius of Kingston, Ontario.
- Gathers listing details including title, price, address, number of bedrooms, number of bathrooms, and date posted.
- Exports the results to an Excel file, with formatting for better readability.

## Requirements

- Python 3.x
- BeautifulSoup4
- Selenium
- Requests
- Pandas
- OpenPyXL

## Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/AatifM/kijiji-student-housing-scraper.git
   cd kijiji-student-housing-scraper

2. **Install the required dependencies:**
   
   ```bash
   pip install requests beautifulsoup4 openpyxl lxml selenium

3. **Run the script**
      
   ```bash
   python main.py

## Output

The scraper will create an Excel file named `kijiji_student_housing.xlsx` containing the scraped listings. The file will have the following columns:

| Column        | Description                                        |
|---------------|----------------------------------------------------|
| `title`       | The title of the listing.                         |
| `price`       | The price of the listing.                         |
| `address`     | The address of the listing.                       |
| `num_bedrooms`| The number of bedrooms.                           |
| `num_bathrooms`| The number of bathrooms.                         |
| `date_posted` | The date when the listing was posted.             |
| `url`         | The URL of the listing.                           |

## Customization

You can modify the script to adjust how it collects data and behaves. Here are a few areas you can customize:

### 1. **Base URL and Search URL**
   - The code will ask you for a URL and you should give it the page you want the listing scraped from.
   - You will have to give it each individual page if there is multiple pages of results and it will generate another file.

   Example:
   ```python
   Enter url: 'https://www.kijiji.ca/' 'https://www.kijiji.ca/b-toronto-on/student-housing/k0l1700273?address=Toronto%2C%20ON&dc=true&ll=43.7%2C-79.42&radius=5.0'
   ```

### 2. **Excel Formatting**
   - Adjust the excel formatting to your liking
