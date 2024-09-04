# LDS General Conference Talk Scraper

This project is a web scraper designed to extract data from the [Latter-day Saint General Conference talks](https://www.churchofjesuschrist.org/study/general-conference?lang=eng) website. The script navigates through the site to gather details from individual conference sessions, including the title, speaker, calling, and content of each talk, along with any associated footnotes. The scraped data is then stored in a CSV file, making it easier to analyze or reference.

## Key Features
- Scrapes conference talks dating back several decades.
- Collects comprehensive data, including talk titles, speakers, callings, content, and footnotes.
- Outputs the data into a structured CSV file, ready for analysis.
- Optional output to JSON format.

## How to Use
1. Clone this repository and open the script in a Python environment, such as Google Colab.
2. Run the script to scrape and store the conference talks.
3. The data will be saved as `conference_talks.csv` and `conference_talks.json`.
4. For long-running tasks, consider saving output files directly to Google Drive to avoid data loss due to session resets.

## Running in Google Colab
- This script can be easily run in Google Colab.
- The scraping process can take anywhere from 30 minutes to an hour to complete, depending on the number of conferences and talks being processed.

## Note
Scraping the entire set of conference talks can be time-consuming. It's recommended to periodically save or download your output files during the process to prevent data loss in case of session interruptions.

