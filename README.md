# TASK-10
📌 Project Overview

This project scrapes real job listings for Data Analyst roles from Internshala using Python + BeautifulSoup, cleans the collected data, and performs basic exploratory analysis.
The project also visualizes the most common job locations and in-demand skills for data analyst positions.

🛠 Tools & Technologies Used

Python 3

Libraries:

requests – Sending HTTP requests

BeautifulSoup – HTML parsing & web scraping

pandas – Data cleaning & analysis

matplotlib – Visualizations

re – Regex for skill cleaning

collections.Counter – Counting skill frequency

📥 Data Collected

From each job listing, the following fields are extracted:

Job Title

Company

Location

Stipend / Salary

Required Skills

The scraper uses User-Agent headers to avoid blocking and introduces delays (time.sleep()) between requests to respect the website.

📊 Analysis Performed
✔ 1. Total Jobs Scraped

Total number of job listings collected across 3 pages.

✔ 2. Top Job Locations

Count of jobs by location.

Visualized using a bar chart.

✔ 3. Most In-Demand Skills

Skills cleaned using regex.

Counted using Counter.

Top 10 skills displayed through a bar chart.

📈 Visuals Generated

Bar Plot: Top 5 job locations

Bar Plot: Top 10 most in-demand skills

These plots help identify trending skills and hotspots for data analyst opportunities.

🧼 Data Cleaning

Removed missing or invalid values

Normalized skills (converted to lowercase, split by comma// etc.)

Handled unstructured text using regex

Ensured clean DataFrame for analysis

⚠️ Challenges Faced

Internshala blocks scraping without proper browser headers

HTML structure changes often → selectors had to be updated

Skills listed inconsistently → required regex & manual cleaning

Some locations and skills missing → handled with fallback values

Added delays (time.sleep(2)) to prevent request blocking

📂 Project Files

job_scraper.ipynb → Full code, scraping, cleaning, analysis, plots

README.md → Project summary (this file)

Plot images (optional)

🎯 Outcome

By completing this project, we successfully:

Scraped real job listings

Performed EDA on job data

Identified trends in skills and locations

Built a reproducible web scraping + analysis workflow

This project demonstrates practical skills in web scraping, data cleaning, analysis, and visualization, which are essential for data analysts and data scientists.
