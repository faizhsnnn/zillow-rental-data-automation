## Zillow Rental Data Automation

This project automates the process of collecting rental property listings and submitting them into a Google Form for data tracking.

The script first scrapes property information from a Zillow-style listings website using BeautifulSoup and Requests. It extracts the property addresses, prices, and listing links.

After collecting the data, Selenium WebDriver is used to automatically fill out a Google Form with the scraped information. Each property listing is submitted as a separate form response.

This project demonstrates how web scraping and browser automation can be combined to build an end-to-end data collection pipeline.

This project was built as part of the #90DaysOfCode challenge to practice web scraping, automation, and data collection workflows using Python.

---

## Technologies Used

Python  
Requests  
BeautifulSoup (bs4)  
Selenium WebDriver  
ChromeDriver

---

## Key Concepts Demonstrated

Web scraping using Requests and BeautifulSoup

Parsing HTML content using CSS selectors

Extracting structured data from web pages

Cleaning and processing scraped text data

Browser automation using Selenium WebDriver

Automating form submission workflows

Combining scraping and automation in a single pipeline

---

## Automation Workflow

1. Send a request to the rental listings website
2. Parse the HTML page using BeautifulSoup
3. Extract property links using CSS selectors
4. Extract and clean property addresses
5. Extract and clean property prices
6. Launch a browser session using Selenium
7. Open a Google Form
8. Automatically fill the form fields with scraped data
9. Submit each property listing as a new form entry

---

## Installation

Install required dependencies

```
pip install requests
pip install beautifulsoup4
pip install selenium
```

Ensure ChromeDriver is installed and compatible with your Chrome browser version.

ChromeDriver should also be accessible via your system PATH.

---

## Run

```
python main.py
```

---

## Configuration

Before running the script, replace the Google Form link in the code:

```
driver.get("YOUR_GOOGLE_FORM_LINK_HERE")
```

Create a Google Form with three fields:

Address  
Price  
Listing Link

Update the XPaths in the script if your form structure differs.

---

## Why This Project Matters

Many real-world workflows require collecting information from websites and storing it in structured systems.

This project demonstrates how Python automation can

Collect data from web pages

Clean and process extracted information

Automatically store data in external platforms

Build end-to-end automation pipelines for data collection

---

## Disclaimer

This project is intended for educational purposes.  
Always respect website terms of service when performing web scraping.

---

## Author

Faiz Hasan  
Python Automation & Backend Developer
