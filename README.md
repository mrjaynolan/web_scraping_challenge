# Mars News and Weather Data Scraping

## Overview

This project involves scraping data from two different Mars-related websites and performing an analysis on the collected data. The project is divided into two parts:

1. **Scrape Titles and Preview Text from Mars News**: Extract the latest news articles from a Mars news website, focusing on the titles and preview texts.
2. **Scrape and Analyze Mars Weather Data**: Scrape Mars weather data, particularly temperature and atmospheric pressure, and perform an analysis to answer key questions about the Martian climate.

### Project Structure

- **part_1_mars_news.ipynb**: Jupyter notebook for scraping Mars news titles and preview texts.
- **part_2_mars_weather.ipynb**: Jupyter notebook for scraping and analyzing Mars weather data.
- **hawaii.sqlite**: SQLite database (included in another example).
- **mars_weather.csv**: CSV file containing the Mars weather data scraped and analyzed in Part 2.
- **README.md**: This file, providing an overview of the project and instructions for running the code.

## Part 1: Scrape Titles and Preview Text from Mars News

### Steps

1. **Automated Browsing and Scraping**:
   - Use Splinter to automate browser actions and visit the Mars news website.
   - Use BeautifulSoup to parse the HTML and extract the necessary elements.

2. **Data Extraction**:
   - Scrape the titles and preview text of the latest news articles.
   - Store each title-preview pair in a Python dictionary with two keys: `title` and `preview`.
   - Store all the dictionaries in a Python list.

3. **Export Data (Optional)**:
   - Optionally, export the list of dictionaries to a JSON file for easier data sharing.

### Requirements

- **Libraries**: Splinter, BeautifulSoup, Pandas, and other necessary Python libraries.
- **Output**: A list of dictionaries containing titles and preview texts.

### Running the Notebook

1. Open the `part_1_mars_news.ipynb` notebook in Jupyter.
2. Run each cell to scrape the data and view the results.
3. Optionally, export the data to a JSON file.

## Part 2: Scrape and Analyze Mars Weather Data

### Steps

1. **Automated Browsing and Scraping**:
   - Use Splinter to automate browsing and visit the Mars Temperature Data Site.
   - Use BeautifulSoup to scrape the data from the HTML table.

2. **Data Cleaning and Analysis**:
   - Assemble the scraped data into a Pandas DataFrame.
   - Ensure the DataFrame columns have the correct headings and data types.
   - Analyze the data to answer the following questions:
     - How many months exist on Mars?
     - How many Martian days' worth of data exist in the dataset?
     - Which month has the lowest and highest average temperature?
     - Which month has the lowest and highest atmospheric pressure?
     - Estimate the number of Earth days in a Martian year.

3. **Visualization**:
   - Create visualizations (bar charts) to support the analysis of temperature and atmospheric pressure.

4. **Export Data**:
   - Export the final DataFrame to a CSV file for future use.

### Requirements

- **Libraries**: Splinter, BeautifulSoup, Pandas, Matplotlib, and other necessary Python libraries.
- **Output**: A CSV file containing the cleaned and analyzed Mars weather data.

### Running the Notebook

1. Open the `part_2_mars_weather.ipynb` notebook in Jupyter.
2. Run each cell to scrape the data, analyze it, and create visualizations.
3. Export the final DataFrame to `mars_weather.csv`.

## Analysis Questions Answered

1. **How many months exist on Mars?**
2. **How many Martian days' worth of data exist in the dataset?**
3. **Which month, on average, has the lowest and highest temperature?**
4. **Which month, on average, has the lowest and highest atmospheric pressure?**
5. **How many Earth days are in a Martian year?**

## How to Use

1. **Setup**:
   - Ensure all necessary Python libraries are installed. You can install them using pip:
     ```bash
     pip install splinter beautifulsoup4 pandas matplotlib
     ```

2. **Run the Notebooks**:
   - Use Jupyter Notebook to open and run the `part_1_mars_news.ipynb` and `part_2_mars_weather.ipynb` notebooks.

3. **Review the Results**:
   - Examine the scraped data, visualizations, and the answers to the analysis questions.

4. **Export the Data**:
   - The cleaned and analyzed Mars weather data will be saved to `mars_weather.csv` after running the notebook.


