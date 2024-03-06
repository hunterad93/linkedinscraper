# Project README

## Overview

I created this for a capstone project but it didn't end up being possible to scrape linkedin at scale without residential proxies. Datacenter proxies were all blacklisted.

This project involves automating various tasks using Selenium and Playwright. The tasks include web scraping, email creation, and PDF parsing. The project is structured into different Jupyter notebooks, each handling a specific task.

### Primary scraping notebook
- `cyborg_testing.ipynb`: This notebook contains functions for creating a Selenium WebDriver with specific user-agent and other settings. It has a series of cells that perform operations, one for logging in, one for bypassing email verification, one for collecting links to scrape and saving them, then finally one to visit each saved link and extract profile.

### Scratch files:

- `protonmailtesting.ipynb`: This notebook handles the automation of tasks related to ProtonMail. It includes creating a DataFrame with account information and extracting verification codes from files.
- `email_creation.ipynb`: This notebook is responsible for automating the process of email creation.
- `parse_pdf.ipynb`: This notebook is used for parsing PDF files. It extracts text from PDF files and saves it to .txt files.
- `playwright_cyborg.ipynb`: This notebook uses Playwright for automating tasks. It includes reading account information from a CSV file and setting up a Playwright browser with specific settings.
- `linked_scraper.ipynb`: This notebook is used for scraping data from LinkedIn. It includes functions for creating a Selenium WebDriver and loading account information from a CSV file.

## Future Work

- Improve browser fingerprinting
- Include proxy rotation