# Explore-Weather-Trends

UDACITY PROJECT:

In this project, I analyzed local and global temperature data.
Compared the temperature trends with my city (San Jose) to overall global temperature trends.

Instructions: Your goal will be to create a visualization and prepare a write up describing the similarities and differences between global temperature trends and temperature trends in the closest big city to where you live. To do this, you’ll follow the steps below:

Extract the data from the database:  There's a workspace in the previous section that is connected to a database. You’ll need to export the temperature data for the world as well as for the closest big city to where you live. You can find a list of cities and countries in the city_list table. To interact with the database, you'll need to write a SQL query. Write a SQL query to extract the city level data. Export to CSV. Write a SQL query to extract the global data. Export to CSV. Open up the CSV in whatever tool you feel most comfortable using. We suggest using Excel or Google sheets, but you are welcome to use another tool, such as Python or R. Create a line chart that compares your city’s temperatures with the global temperatures. Make sure to plot the moving average rather than the yearly averages in order to smooth out the lines, making trends more observable (the last concept in the previous lesson goes over how to do this in a spreadsheet). Make observations about the similarities and differences between the world averages and your city’s averages, as well as overall trends. Here are some questions to get you started. Is your city hotter or cooler on average compared to the global average? Has the difference been consistent over time? “How do the changes in your city’s temperatures over time compare to the changes in the global average?” What does the overall trend look like? Is the world getting hotter or cooler? Has the trend been consistent over the last few hundred years? Submission Your submission should be a PDF that includes:

An outline of steps taken to prepare the data to be visualized in the chart, such as: What tools did you use for each step? (Python, SQL, Excel, etc) How did you calculate the moving average? What were your key considerations when deciding how to visualize the trends? Line chart with local and global temperature trends At least four observations about the similarities and/or differences in the trends Rubric A Udacity reviewer will assess your project based on the criteria in the project rubric. Use the rubric as a guide while you complete the project, then give yourself a quick self-assessment before you submit it.

If you're on this page, then you should have completed your exploration of local and global temperature trends. Congratulations! Before you submit your project, make sure to check the following points:

Please submit your project as a PDF. Your report should include documentation of the steps in your analysis, a line chart depicting the local and global temperature data, and your observations regarding the trends. Don't forget to review the rubric! Reviewers will use the rubric to assess your work, so make sure it 'meets specifications' on all points before you submit. Once you've checked the above, click on the "Submit Project" button below to go to the project submission page. After you submit your project, it can take up to a week for it to be evaluated. Most of the time, it is much faster! In the meantime, you can feel free to continue to other parts of the program to continue your learning!


Extracted data from SQL workspace and downloaded the results to a CSV file:

Here are the data queries

1. This contains the average global temperatures by year.

SELECT * 

FROM global_data;

2. This contains the average temperatures for each city by year.

SELECT * 

FROM city_list

WHERE city = 'San Jose';

3. This contains a list of cities and countries in the database. So extracted my neaest city 'San Jose' from the data.

FROM city_data

WHERE city = 'San Jose';


# Observations:

1. The global temperature has been in the range of 8 °C and 10 °C in the time period 1849 - 2013, Whereas San Jose City temperature has been hotter, in the range of 14 °C and 16 °C at the same time period.

2. San Jose city recored its lowest average temperature of 13.2 °C in 1860 and 16.2 °C as highest avg temperature in year 2013.

3. The lowest global average temperature of 7.5 °C was recorded in the year 1862 and the highest global average temperature of 9.7 °C was recorded in the year 2007. 

4. The difference between global and San Jose average temperatures looks to be steadily decreasing (from 6.3 °C to 5.7 °C) from 1870 up till 1930 as San Jose was getting slightly colder and earth was slightly getting warmer.

5. In the last 2 years (2011 - 2013) San Jose city temperature seem to be increasing at a much higher rate (0.85 °C per year), where as the global average temperature was almost constant.

6. The overall trend looks like the world is getting hotter, throughout the time period
