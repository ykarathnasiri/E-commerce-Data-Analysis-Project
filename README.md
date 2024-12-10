
# E-commerce Purchase Analysis and Web Scraping Project

This project combines exploratory data analysis (EDA) of sample e-commerce purchase data with a web scraping component to enrich the analysis with real-world product data. It demonstrates data manipulation, visualization, and web scraping techniques using Python libraries like Pandas, Matplotlib, Seaborn, Beautiful Soup, and Requests.

## Project Overview

The project consists of two main parts:

1. **E-commerce Purchase Analysis:** EDA is performed on a sample dataset (`purchase_data.csv`) containing customer purchases, including product categories, amounts, and timestamps. The analysis includes descriptive statistics, monthly sales calculations, product category performance analysis, and customer purchase insights.  Visualizations such as sales trend charts, category purchase count bar charts, and revenue distribution pie charts are generated.

2. **Web Scraping from ikman.lk:** The project scrapes product data from the Sri Lankan classifieds website ikman.lk.  It extracts product titles, links, membership status (premium/non-premium, verified/non-verified), location, category, price, ad type (top ad/normal ad), and image URLs. The scraped data is saved to a CSV file (`ikman_data.csv`) and then cleaned and preprocessed.  Further EDA is performed on this scraped data including price analysis and visualization and an analysis of member types.  Finally, the scraped data is integrated with the original purchase data for a combined analysis.

## Setup Instructions

1. **Clone the Repository:** Clone this repository to your local machine using:

   ```bash
   git clone https://github.com/ykarathnasiri/E-commerce-Data-Analysis-Project.git 
   ```

2. **Create a Virtual Environment (Recommended):** Create a virtual environment to isolate project dependencies.

   ```bash
   python3 -m venv .venv  # Or use your preferred method (conda, virtualenvwrapper, etc.)
   source .venv/bin/activate  # Activate the environment (Linux/macOS)
   .venv\\Scripts\\activate  # Activate the environment (Windows) 
   ```

3. **Install Dependencies:** Install the required Python libraries using `pip`:

   ```bash
   pip install -r requirements.txt
   ```
   or
   ```bash
   pip install pandas numpy matplotlib seaborn beautifulsoup4 requests openpyxl tqdm
   ```


4. **Run the Jupyter Notebook:** Open and run the Jupyter notebook (`E-commerce Data Analysis Project.ipynb`).  

   ```bash
   jupyter notebook E-commerce Data Analysis Project.ipynb 
   ```
   The notebook contains detailed explanations and code for each step of the project.


## Data

* **purchase_data.csv:**  A sample CSV file containing e-commerce purchase data. This file is created by the notebook itself.
* **ikman_data.csv:** The raw scraped data from ikman.lk, also created by the notebook.
* **ikman_data_cleaned.csv:** The cleaned and preprocessed version of the scraped data.
* **sales_analysis.xlsx:**  Excel file containing the filtered/summarized data from the purchase dataset. Created by the notebook upon execution of relevant cells.
* **merged_dataset.csv:** CSV file containing the merged data from the sample purchase data and the scraped Ikman data. Created by the notebook.

## Project Details and Enhancements

* **Web Scraping:** The scraping component can extract data from multiple pages of ikman.lk based on a user-defined query and number of pages. It handles membership information and ad types, providing a comprehensive dataset. Error handling for web requests could be further enhanced to make the scraper more robust (e.g., handling timeouts, HTTP errors, and page changes).
* **Data Cleaning:** The notebook includes data cleaning steps to handle missing values and format numerical columns correctly.  More advanced cleaning and data validation could be implemented depending on the specific needs of the analysis.
* **Exploratory Data Analysis:** The notebook provides a variety of analyses and visualizations to gain insights from both the sample purchase data and the scraped data. More complex analyses (e.g., time series analysis, customer segmentation) can be added to delve deeper into the data.
* **Data Integration:** The scraped product data from ikman.lk is combined with the initial sales dataset, allowing for explorations of relationships between the two (e.g., identifying popular products, analyzing pricing trends).
* **Custom Analytics Features:** The notebook includes a search function to retrieve purchases by a specific customer, a filter function to find purchases within a date range or exceeding a given amount, and a function to calculate the total revenue for a specific product category.  These interactive features make the analysis more dynamic and user-friendly.
* **Excel Export (Bonus):** The project exports the filtered and summarized data into an Excel file for further analysis or reporting.

## Further Exploration

* **Advanced Visualizations:** Implement more sophisticated visualizations to explore patterns and trends in the data.
* **Statistical Modeling:**  Apply statistical models to predict future sales or customer behavior.
* **Interactive Dashboard:** Create an interactive dashboard to dynamically explore and visualize the data.


This project provides a foundation for more extensive e-commerce analytics. By adapting the web scraping component and extending the analysis, you can gain valuable insights into diverse e-commerce datasets.

