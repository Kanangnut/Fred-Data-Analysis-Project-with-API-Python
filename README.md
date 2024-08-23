## Fred-Data-Analysis-Project-with-API-Python

This project is focused on analyzing economic data using the FRED API, which provides access to a wealth of economic data from the Federal Reserve Bank of St. Louis. The key steps in the project are:

1. **API Setup**: The project begins by loading a secret API key from a JSON file to interact with the FRED API. The API key is essential for accessing the data.

2. **FredPy Class**: A custom Python class `FredPy` is created to manage interactions with the FRED API. This class includes methods to set the API token and to fetch economic data series based on specific parameters such as `seriesID`, date range, and units.

3. **Fetching Data**: The project retrieves two specific economic data series:
   - **GDP (Gross Domestic Product)**: Data from January 2005 to December 2021, presented as a percentage change (annualized).
   - **Unemployment Rate**: Data from the same period, presented as a linear percentage.

4. **Data Processing**: The data fetched from the API is converted into a Pandas DataFrame, with dates parsed into a datetime format and values converted to floats for further analysis.

5. **Visualization**: The project concludes with visualizing the GDP and Unemployment Rate data on a single plot, showing trends over the specified period. The plot is labeled appropriately, with a title, axis labels, and a legend to distinguish the two data series.

This project provides a foundation for analyzing and visualizing economic indicators, useful for understanding economic trends and making informed decisions based on historical data.

### Tools Used:
1. **Python**: The primary programming language used for scripting, data processing, and visualization.
2. **Pandas**: A Python library used for data manipulation and analysis. It's utilized to create DataFrames, handle date conversions, and manage data types.
3. **Matplotlib**: A plotting library in Python used to visualize the economic data (GDP and Unemployment Rate) in a time-series plot.
4. **FRED API**: An API provided by the Federal Reserve Bank of St. Louis to access a wide range of economic data. It's used to retrieve GDP and Unemployment Rate data.

### Technical Concepts:
1. **API Integration**: The project demonstrates how to integrate with a RESTful API (FRED API) using Python's `requests` library. It involves forming URL requests with the appropriate parameters and handling JSON responses.

2. **Class-Based Design**: The `FredPy` class encapsulates API interactions, making it easy to reuse and extend for fetching different economic data series. This design promotes modularity and code reuse.

3. **Data Processing**: The project showcases essential data processing techniques:
   - Converting JSON data into a Pandas DataFrame.
   - Parsing and formatting dates using `pd.to_datetime`.
   - Handling numeric data by converting strings to floats for analysis.

4. **Data Visualization**: The project uses Matplotlib to create a line plot that visually compares two economic indicators over time. This includes adding titles, labels, legends, and customizing the plot's appearance.

5. **Error Handling**: The project includes basic error handling, checking for successful API responses and raising exceptions if the API key is missing or the response is unsuccessful.
