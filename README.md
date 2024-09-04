
# General Conference Talk Scraper

This project is a web scraper designed to extract and clean data from the [General Conference talks](https://www.churchofjesuschrist.org/study/general-conference?lang=eng) website for The Church of Jesus Christ of Latter-day Saints. The script navigates through the site to gather details from individual conference sessions, including the title, speaker, calling, and content of each talk, along with any associated footnotes. The data is then cleaned to ensure consistency and saved in a structured CSV file for easy analysis.

## Key Features
- **Scraping**: Gathers conference talks dating back several decades.
- **Data Collection**: Extracts talk titles, speakers, callings, content, and footnotes.
- **Data Cleaning**: Standardizes the data by:
  - Removing non-talk rows (e.g., session headings, "Church Auditing Department" rows).
  - Standardizing callings (e.g., "Quorum of the 12" and "Seventy").
  - Removing speaker titles such as "Elder," "President," etc.
- **Output Formats**: Saves the data in both CSV and JSON formats, ready for analysis.

## How to Use
1. Clone this repository and open the script in a Python environment, such as Google Colab.
2. Run the script to scrape, clean, and store the conference talks.
3. The cleaned data will be saved as `cleaned_conference_talks.csv` and `conference_talks.json`.
4. For long-running tasks, consider saving output files directly to Google Drive to avoid data loss due to session resets.

## Running in Google Colab
- This script can be easily run in Google Colab.
- The scraping and cleaning process can take anywhere from 30 minutes to an hour to complete, depending on the number of conferences and talks being processed.

## Data Cleaning
After scraping, the data undergoes several cleaning operations:
- Removal of session heading rows (e.g., morning/afternoon/evening sessions).
- Removal of rows related to "Church Auditing Department" or non-talk content.
- Standardization of callings like "Quorum of the 12" and "Seventy."
- Removal of speaker titles such as "Elder," "President," "Sister," etc.
- The cleaned data is saved in `cleaned_conference_talks.csv`.

## Note
Scraping and cleaning the entire set of conference talks can be time-consuming. It's recommended to periodically save or download your output files during the process to prevent data loss in case of session interruptions.

## Acknowledgments
This code is based on the original work found in the [LDS Conference Scraper](https://github.com/johnmwood/LDS-Conference-Scraper) GitHub repository by [johnmwood](https://github.com/johnmwood).
"""
