# Naukri Web Scraping

🚀 Welcome to the Naukri Web Scraping Project! This project involves scraping job listings from Naukri.com, extracting valuable information, cleaning and processing the data, and creating insightful visualizations using Tableau. Below, you'll find an overview of the project, its prerequisites, execution steps, and a brief description of the analysis and dashboard creation.

## 📝 Project Overview

The goal of this project is to collect job data from Naukri.com using web scraping techniques, process the data, and analyze it to gain meaningful insights about job listings, companies, locations, skills, and more. The project is divided into two main parts:

1. **Web Scraping:** In this phase, we utilize Selenium and Beautiful Soup to extract job listings from Naukri.com. The data extracted includes job title, rating, company, reviews, salary, location, skills, and more. Each page's data is parsed using an HTML parser, and a user-defined function is employed to convert the parsed data into a DataFrame. All DataFrames are appended to a list and concatenated into a single CSV file named `raw_cleaned_data.csv`.

2. **Analysis and Dashboard:** The collected data is imported into Tableau for analysis and visualization. Various visualizations are created to highlight insights about job locations, job titles, required skills, and top recruiters. The final dashboard is designed for interactive exploration of the data.

## 🛠 Prerequisites

Before running the project, ensure you have the following installed:

- Python with pip
- Beautiful Soup 4 (`pip install bs4`)
- Selenium (`pip install selenium`)
- Google Chrome Driver
- Tableau (for analysis and dashboard creation)

## ⚙ Execution Steps

1. Clone this repository to your local machine.

2. Download and place the Google Chrome Driver executable in the appropriate directory.

3. Run the web scraping script (`Naukri.py`) to collect job data from Naukri.com.

4. Run the Tableau workbook to connect the generated CSV files (`raw_cleaned_data.csv`, `loc_table.csv`, `skills_table.csv`) and create visualizations.

## 📊 Analysis and Visualization

The analysis and visualization part is carried out in Tableau:

- A location map is created, where the size of each location dot corresponds to the count of jobs in that location.

- A tree map visualization showcases different job titles or roles, emphasizing the distribution of job listings.

- Required skills for each job title are presented, shedding light on the skills in demand.

- Top recruiters for each job section are identified and highlighted.

All visualizations, except for the location map, are parameter-controlled to allow dynamic exploration.

For more detailed information and to interact with the final dashboard, check out the [Tableau Public Dashboard](https://public.tableau.com/app/profile/anshid.t.k/viz/Naukriblended/Naukridashboard).

Happy coding! 🌟👩‍💻👨‍💻

> Note: Ensure that you respect Naukri.com's terms of use and follow ethical web scraping practices while collecting data.
