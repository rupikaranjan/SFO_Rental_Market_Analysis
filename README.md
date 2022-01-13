# SFO_Rental_Market_Analysis
    This data visualization application analysis the housing rental market data in San Francisco area and helps the user to find properties that are viable investment for them. 
    
---

## Technologies

This application works on python 3.7 and uses following libraries:

* [hvplot](https://pyviz-dev.github.io/hvplot/index.html) - A component of PyViz ecosystem used for creating Interactive Visualizations of data.
* [geoviews](https://github.com/holoviz/geoviews) - A component of PyViz ecosystem used for visualization of geospacial(location-based) data.

---

## Installation Guide

Follow the following instructions before using the application.

```python 
  conda install -c pyviz hvplot geoviews
```
---

### Calculate and plot the housing units per year

 Using numerical and visual aggregation, we calculate the number of housing units per year, and then visualize the results as a bar chart.

    1. Using `groupby` function to group the data by year and the `mean` of the result is calculated.

    2. Using the `hvplot` function to plot the `housing_units_by_year` DataFrame as a bar chart
    
    ![housing_unit_bar_chart](Resources/Images/housing_unit_bar_chart.png)
    
    ![question1](Resources/Images/question1.png)
    
---

## Calculate and Plot the Average Sale Prices per Square Foot

Using numerical and visual aggregation, we calculate the average prices per square foot, and then visualize the results as a line plot.


    1. The data is grouped by year using `groupby` function and the `mean` of the result is calculated.

    2. A new dataframe `prices_square_foot_by_year` is created by filtering out the “housing_units” column and including just the averages per year for only the sale price per square foot and the gross rent.

    3. A line plot of the `prices_square_foot_by_year` is plotted using `hvplot` function with `year` in x-axis and both `sale_price_sqr_foot` &  `gross_rent` in y-axis. The plot is then formatted and styled.

    ![prices_square_foot_by_year_plot](Resources/Images/prices_square_foot_by_year_plot.png)

    ![question2](Resources/Images/question2.png)
    

