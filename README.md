This project is focused on analyzing economic data using the FRED API, which provides access to a wealth of economic data from the Federal Reserve Bank of St. Louis. The key steps in the project are:

1. **API Setup**: The project begins by loading a secret API key from a JSON file to interact with the FRED API. The API key is essential for accessing the data.

2. **FredPy Class**: A custom Python class `FredPy` is created to manage interactions with the FRED API. This class includes methods to set the API token and to fetch economic data series based on specific parameters such as `seriesID`, date range, and units.

3. **Fetching Data**: The project retrieves two specific economic data series:
   - **GDP (Gross Domestic Product)**: Data from January 2005 to December 2021, presented as a percentage change (annualized).
   - **Unemployment Rate**: Data from the same period, presented as a linear percentage.

4. **Data Processing**: The data fetched from the API is converted into a Pandas DataFrame, with dates parsed into a datetime format and values converted to floats for further analysis.

5. **Visualization**: The project concludes with visualizing the GDP and Unemployment Rate data on a single plot, showing trends over the specified period. The plot is labeled appropriately, with a title, axis labels, and a legend to distinguish the two data series.

This project provides a foundation for analyzing and visualizing economic indicators, useful for understanding economic trends and making informed decisions based on historical data.
