# Data-Analysis-on-Audible-Dataset

## Project Overview
This project performs data cleaning and analysis on an Audible dataset, which includes details of around 87,489 audiobooks. The dataset provides information on audiobook names, authors, narrators, duration, release dates, ratings, and pricing, allowing me to explore trends and gain insights into user preferences on the Audible platform.

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Setup Instructions](#setup-instructions)
- [Notebook Structure](#script-structure)
- [Data Cleaning Process](#data-cleaning-process)
- [Data Analysis](#data-analysis)
- [Insights](#insights)

## Dataset
The dataset includes details such as:
- **name**: The title of each audiobook.
- **author**: The author of each audiobook, prefixed with "writtenby".
- **narrator**: The narrator of each audiobook, prefixed with "Narratedby".
- **time**: Duration of each audiobook in hours and minutes.
- **release date**: The release date of each audiobook.
- **rating**: User ratings for each audiobook.
- **total ratings**: Number of ratings received by each audiobook.
- **price**: Price of each audiobook.

## Setup Instructions
1. Clone this repository:
   ```bash
   git clone https://github.com/arafayr/audible-data-analysis.git
   ```

2. Install the required libraries:
   ```bash
   pip install pandas numpy word2number
   ```

3. Make sure `audible_uncleaned.xlsx` is in the same directory as the script or update the file path accordingly in `data_analysis_audible.ipynb`.


## Notebook Structure
The `data_analysis_audible.ipynb` notebook performed following tasks on Audible dataset:

1. **Data Loading**:
   - The dataset is loaded from an Excel file using `pandas`.
   
2. **Data Inspection**:
   - Displaying the initial shape and a preview of the data.
   - Basic data summary and column descriptions for a better understanding of the dataset.

3. **Data Cleaning**:
   - Steps to handle missing values and clean text data, such as removing prefixes like "writtenby" and "Narratedby" from author and narrator fields.
   - Conversion of duration strings into a numeric format for consistency.
   - Parsing and standardizing date formats for consistency in the `release date` column.
   - Handled missing values, ensuring the dataset is complete and ready for analysis.
   - and more... 
   
4. **Data Analysis**:
   - Descriptive statistics for numerical columns (e.g., ratings, prices etc).
   - Analysis of audiobook duration and patterns in relation to ratings and prices.
   - Insights into the distribution of audiobooks based on their release dates.
   - Analysis on top-rated authors, narrators, and the price ranges of audiobooks.
   - Examined audiobook prices to understand the distribution and common price ranges.

## Insights
Key insights from the analysis include:
- Relationships between audiobook length, rating, and price.
- Popular genres or categories on the Audible platform.
- Distribution patterns for ratings and pricing across audiobooks.
