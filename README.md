# FreezeEffect-TrackAndField-Records
Repository for tracking Freeze Effect Track and Field results

## Repository Structure

* **`TeamName_TrackAndField_Records/`**: The top-level directory for your team's entire data repository.
* **`[Year]_Season/`**: Each season has its own folder to keep results organized by year.
* **`[YYYY-MM-DD]_MeetName/`**: Subfolders within each season for specific meets, named with the date and meet title for clear chronological ordering.
    * **`full_results.csv`**: A file containing all results from a particular meet. Using the **CSV format** makes the data easy to read and parse.
    * **`individual_results/`**: A subdirectory for individual athlete results, with each file named for the athlete and event (e.g., `JaneDoe_100m.csv`).
* **`Historical_Records/`**: This directory is for all-time team and individual records.
    * **`team_records.csv`**: A central file for team-wide records (e.g., relay records, team points).
    * **`individual_records/`**: Subfolders or files for specific event records, making it easy to see the top performers in each discipline.
* **`Scripts/`**: This is a key part of an automated system. Store any code here that helps you **extract, parse, or update** your data.
    * `extract_results.py`: A script for web scraping or downloading results from official meet websites.
    * `parse_data.py`: A script to clean and format raw data into a usable structure.
    * `update_records.py`: A script that automatically compares new results against existing historical records and updates them if a new record is set.
* **`README.md`**: This document provides an overview of the repository structure and instructions on how to use it.
* **`.gitignore`**: A file to tell Git to ignore certain files and folders, like temporary files or sensitive data.
