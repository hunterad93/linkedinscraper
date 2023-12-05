# Project README

## Overview

I created this for a capstone project but it didn't end up being possible to scrape linkedin at scale without residential proxies. Datacenter proxies were all blacklisted.

This project involves automating various tasks using Selenium and Playwright. The tasks include web scraping, email creation, and PDF parsing. The project is structured into different Jupyter notebooks, each handling a specific task.

## Codebase Structure

Note: cyborg_testing is the most maintained and workable code.

- `protonmailtesting.ipynb`: This notebook handles the automation of tasks related to ProtonMail. It includes creating a DataFrame with account information and extracting verification codes from files.
- `cyborg_testing.ipynb`: This notebook contains functions for creating a Selenium WebDriver with specific user-agent and other settings.
- `email_creation.ipynb`: This notebook is responsible for automating the process of email creation.
- `parse_pdf.ipynb`: This notebook is used for parsing PDF files. It extracts text from PDF files and saves it to .txt files.
- `playwright_cyborg.ipynb`: This notebook uses Playwright for automating tasks. It includes reading account information from a CSV file and setting up a Playwright browser with specific settings.
- `linked_scraper.ipynb`: This notebook is used for scraping data from LinkedIn. It includes functions for creating a Selenium WebDriver and loading account information from a CSV file.

## Setup

1. Install the required Python packages: Selenium, Playwright, pandas, PyPDF2, and others.
2. Update the account information in the respective notebooks (`protonmailtesting.ipynb`, `playwright_cyborg.ipynb`, `linked_scraper.ipynb`).
3. Run the notebooks.

## Note

- The .gitignore file is set to ignore .txt, .pdf, .csv, and .ovpn files. Make sure to not commit sensitive data.
- The project uses specific user-agents and proxies. Update these as per your requirements.
- The project uses specific file paths for reading and writing data. Update these paths as per your system's directory structure.

## Future Work

- Refactor the code to remove redundancy.
- Improve error handling and add logging for better debugging.
- Consider using a database for storing account information instead of CSV files.