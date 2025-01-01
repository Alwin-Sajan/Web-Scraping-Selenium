# Selenium with Python - Workshop

This repository contains the Jupyter Notebook used during the workshop to demonstrate how to automate web browsers using the Selenium WebDriver with Python.

## Workshop Overview

This workshop covers the basics of Selenium WebDriver and its integration with Python to perform web scraping, browser automation, and testing. By the end of this workshop, you'll have a solid understanding of:

- How to install and set up Selenium WebDriver.
- How to interact with web elements using Python.
- How to perform basic automation tasks (e.g., filling out forms, clicking buttons).
- Techniques for scraping dynamic web content.
- Writing basic test scripts for web applications.

## Prerequisites

Before starting the workshop, you need to have the following installed:

1. **Python** (version 3.6 or higher) - [Download Python](https://www.python.org/downloads/)
2. **Jupyter Notebook** - [Install Jupyter](https://jupyter.org/install)
3. **Selenium** - Install via pip:
   ```bash
   pip install selenium
   ```
4. **WebDriver** - Download the appropriate WebDriver for your browser:
   - [ChromeDriver](https://sites.google.com/a/chromium.org/chromedriver/downloads)
   - [GeckoDriver](https://github.com/mozilla/geckodriver/releases) (for Firefox)
   - Ensure the WebDriver executable is in your system's PATH or specify its path in your code.

## Repository Structure

The repository contains the following files:

- **`Web Scraping - CoreAI ppt.pdf`**: It is the ppt used in the workshop .
- **`bookPrice.ipynb.ipynb`**: This is the book price Jupyter Notebook used during the workshop.
- **`books_data.csv`**: It contain the output which is books price in csv format

## Running the Jupyter Notebook

To run the notebook:

1. Clone this repository:
   ```bash
   git clone https://github.com/Alwin-Sajan/Web-Scraping-Selenium.git
   ```

2. Navigate to the directory:
   ```bash
   cd Web-Scraping-Selenium
   ```

3. Launch Jupyter Notebook:
   ```bash
   jupyter notebook
   ```

4. Open the `bookPrice.ipynb.ipynb` file in the Jupyter Notebook interface.

5. Follow along with the instructions and code in the notebook.

## Key Topics Covered

- **Setting up Selenium WebDriver**: How to install and configure Selenium for different browsers.
- **Interacting with Web Elements**: Locating elements using various Selenium locators (e.g., `id`, `name`, `xpath`, `css selector`).
- **Automation**: Automating form submission, clicking buttons, navigating between pages, and handling alerts.
- **Web Scraping**: Extracting data from dynamically-loaded content.
- **Handling Waits**: Dealing with waiting for elements to load using explicit and implicit waits.
- **Testing**: Writing simple automated tests for web applications.

## Example Usage

```python
from selenium import webdriver
from selenium.webdriver.common.by import By

# Initialize the WebDriver
driver = webdriver.Chrome()

# Open a webpage
driver.get("https://www.example.com")

# Find an element and interact with it
search_box = driver.find_element(By.NAME, "q")
search_box.send_keys("Selenium with Python")
search_box.submit()

# Close the WebDriver
driver.quit()
```

