# Web Scraping Top Data Firms
## [View Full Project](https://nbviewer.org/github/TelRich/Data-Analytics-Company-Web-Scraping/blob/main/top_da_company.ipynb)

![](newplot.png)

### Summary

* The webpage from Goodfirm was succesfully accessed and downloaded using Request library. 
* BeautifulSoup was used to locate and extract the details from the downloaded html file
* The extracted details was converted to data frame using Pandas.
* The file was cleaned and changed to its right datatype
* The cleaned file was explored for some insights.

#### Findings
* About 30 firms are rated 5 star while 12 are rated between 4.8 - 4.9
* Very few firms (3) has a review above 30
* Most of the firms are located in United States followed by India.

## My contributions:

# Web Scraping: Top Data Analytics Firms

This project is an automated data extraction tool designed to gather strategic information about leading data analytics companies.

## New Features
The capabilities of the original script have been extended by creating custom functions in `functions.py` to extract:

* **Website URLs**: Captures direct links to official pages by accessing the `href` attribute.

* **Email Addresses**: Extracts and cleans contact addresses by removing the `mailto:` prefix for direct use in databases.

* **Geographic Data and Names**: Organizes location information and names of firms.

## Technical Implementation Details
Unlike simple text extraction, the new features implement:
1. **Access to Attributes**: Uses `tag['href']` to obtain paths that are not visible as plain text.

* 2. **Data Cleaning**: Using the `.replace()` method to normalize email addresses.

3. **Pandas Integration**: Data is returned as `pd.Series` to facilitate export to CSV files or SQL databases.

## Requirements
* Python 3.x
* Pandas
* BeautifulSoup4