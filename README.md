### Introduction

The goal of this project is to:

-Extract relevant text and media data from public Telegram channels focused on Ethiopian medical businesses.
-Store raw data for preprocessing and analysis.
-Perform data cleaning and transformation for further analysis.

### Methodology


Telegram Scraping with Telethon
We use Telethon to interact with Telegram's API, allowing us to scrape public channels like EAHCI and other relevant channels.
The scraper.py script handles connecting to Telegram, extracting messages and media, and storing them in a local database for further processing.
Data Storage
Raw data is temporarily stored in a SQLite database or local files for initial storage.
After cleaning, the data is stored in a structured PostgreSQL database for further analysis.
Logging
Python's logging module is used to track the scraping process, log errors, and monitor progress.
Data Cleaning
The data cleaning process includes:

Removing duplicates: Any duplicate messages or media are removed.
Handling missing values: Missing values are either filled with default values or removed.
Standardizing formats: All data is standardized for consistency, such as formatting timestamps and product names.
