
<h1 align="center">Bay Area Housing Market Insights &amp; Visualization</h1>

<p align="center">
  <img src="Housing%20market%20dashboard%20screenshot.png"
       alt="Bay Area Housing Market Power BI Dashboard"
       width="700">
</p>
<p align="center">
  <strong>Python | Google BigQuery | Power BI | Data Preparation | Data Visualization</strong>
</p>

## Project Overview

This project explores residential housing market conditions in the San Francisco Bay Area through data collection, preparation, integration, and interactive visualization.

Developed as part of **DSC 540 – Data Preparation at Bellevue University**, the project combines residential property listing information with economic indicators to examine housing prices, property characteristics, and broader market conditions.

The project demonstrates Python-based data collection and preparation, Google BigQuery connectivity, and interactive dashboard development using Microsoft Power BI.

## Project Objectives

- Analyze residential housing prices and property characteristics across Bay Area communities.
- Explore relationships between sales prices, square footage, bedrooms, bathrooms, and year built.
- Incorporate economic indicators, including labor force, income, and the Consumer Price Index (CPI).
- Develop interactive visualizations to support housing market exploration.
- Demonstrate data collection, cleaning, transformation, and visualization techniques.

## Technologies and Tools

| Technology | Purpose |
|---|---|
| Python | Data collection, cleaning, and preparation |
| pandas / NumPy | Data manipulation and transformation |
| Requests | API-based data retrieval |
| RentCast API | Residential property listing information |
| pdfplumber | Extraction of data from PDF documents |
| Google BigQuery | Cloud data source accessed by Power BI |
| Microsoft Power BI | Interactive data visualization and reporting |
| Jupyter Notebook | Python development and documentation |

## Data Sources

The project incorporates information from several sources:

- **RentCast API:** Residential property listings and housing characteristics.
- **Alameda County labor force data:** Employment-related economic information.
- **California Consumer Price Index:** Consumer price and inflation indicators.
- **Historical income data:** Economic information used to explore housing market conditions.

## Data Collection and Preparation

Python was used to collect, clean, and prepare housing and economic datasets.

The available notebook documents activities including:

1. Retrieving residential property listings through the RentCast API.
2. Importing economic data from external sources.
3. Cleaning and restructuring data using pandas.
4. Identifying duplicate housing records.
5. Preparing property attributes for analysis.
6. Exporting cleaned datasets for subsequent processing.

The Power BI report accesses a prepared housing dataset stored in Google BigQuery.

**Note:** The repository includes the available Python data collection and preparation notebook. The original code used to load the combined dataset into BigQuery is not included.

## Power BI Dashboard and Visualizations

The Power BI dashboard provides an interactive view of Bay Area residential property information and economic indicators.

### Dashboard Highlights

- **7,157 housing records** represented in the project dashboard.
- **13 cities** included in the housing dataset.
- Minimum recorded sale price of **$5,500**.
- Maximum recorded sale price of **$7.3 million**.
- Interactive filters for location and property characteristics.
- Sales price comparisons by square footage, bedrooms, bathrooms, and year built.
- Visualizations incorporating CPI, income, and housing price indicators.
- Property-level information for detailed exploration.

These figures describe the original project dataset and do not represent current housing market conditions.

### Dashboard Preview

The dashboard screenshot displayed directly beneath the project title provides a static preview of the original Power BI report.

The complete Power BI file is available in this repository for users who wish to explore the interactive visualizations.

## Project Files

| File | Description |
|---|---|
| [Python Data Preparation Notebook](Clindsey_Wk5_6_Project_Milestone3_for_github.ipynb) | Python code for housing data retrieval, cleaning, and preparation |
| [Power BI Report](Final%20Project%20Deliverable.pbix) | Original interactive Power BI dashboard |
| [Dashboard PDF Preview](clindsey_PBI_Visualization_Milestone5.pdf) | Static PDF screenshot of the Power BI dashboard |
| [Dashboard Screenshot](Housing%20market%20dashboard%20screenshot.png) | PNG image displayed beneath the project title |

## How to Run the Python Notebook

The Python notebook uses the RentCast API to retrieve residential property listing information.

### Obtaining Your Own API Credentials

To execute the API-dependent portions of the notebook:

1. Visit [RentCast](https://www.rentcast.io/).
2. Create an account and obtain an API key through the available developer services.
3. Download the Python notebook from this repository.
4. Install the Python libraries required by the notebook.
5. Locate the API authentication section:

    ```python
    headers = {
        'Accept': 'application/json',
        'X-Api-Key': ''
    }
    ```

6. Replace the empty string with your own valid RentCast API key.
7. Execute the API-dependent cells to retrieve housing data.

### API Access and Execution Notes

- Personal API credentials have been intentionally excluded from the public notebook.
- RentCast API access may be subject to subscription fees or usage limits.
- Current API responses may differ from the original project dataset because residential property listings change over time.
- Additional local source files may be required to reproduce some economic-data preparation steps.
- The notebook contains previously saved execution results, allowing visitors to review the original outputs without rerunning the code.

**Security Reminder:** Do not publish personal API keys or other private credentials in a public GitHub repository.

## Google BigQuery Integration

The Power BI report connects to the following Google BigQuery table:

`cris-project-394423.DSC540.CombinedHousingData`

The report uses this SQL query to retrieve the prepared dataset:

```sql
SELECT *
FROM `cris-project-394423.DSC540.CombinedHousingData`
```

The original BigQuery environment is not publicly accessible through this repository.

Users wishing to refresh the Power BI report must configure an accessible data source and appropriate Google Cloud credentials.

The original script used to load the combined dataset into BigQuery is not included in this repository.

## Viewing the Power BI Dashboard

### Option 1: View the Dashboard Screenshot

The dashboard screenshot is displayed directly below the project title.

Visitors can also open the PDF preview to examine the completed visualization without installing Power BI.

### Option 2: Open the Interactive Power BI Report

1. Download `Final Project Deliverable.pbix`.
2. Open the file using Microsoft Power BI Desktop.
3. Explore the available report pages, visualizations, and filters.

Refreshing the original BigQuery data connection requires separate authorization.

## Skills Demonstrated

- Python programming
- REST API data retrieval
- Data cleaning and transformation
- Multi-source data preparation
- Data quality assessment
- Google BigQuery connectivity
- Power BI dashboard development
- Exploratory data analysis
- Interactive data visualization
- Housing market and economic indicator analysis

## Project Information

**Project:** Bay Area Housing Market Insights & Visualization  
**Course:** DSC 540 – Data Preparation  
**Institution:** Bellevue University  
**Author:** Criselvi Lindsey

---

*This repository showcases an academic data preparation and visualization project. Historical results are provided for educational and professional portfolio demonstration purposes.*
