Deliverable 1: Scrape titles and preview text from Mars news articles.
Create a new Jupyter notebook named mars_data_challenge_part_1.ipynb.

Scrape the Mars NewsLinks to an external site. website by using Splinter and Beautiful Soup. Specifically, scrape the title and preview text, or summary text, of each article on the landing page.

Store the scraping results in Python data structures as follows:

. Store each title-and-preview pair in a Python dictionary. And, give each dictionary two keys: title and preview. An example is the following:

. {'title': "Mars Rover Begins Mission!", 'preview': "NASA's Mars Rover begins a multiyear mission to collect data about the little-explored planet."} Store all the dictionaries in a Python list.

. Print the list in your notebook.

Deliverable 2: Scrape and analyse Mars weather data, which exists in a table.
Created a Jupyter notebook named mars_data_challenge_part_2.ipynb. Import the relevant dependencies for web scraping, Pandas, and Matplotlib.

automated browser, visit the Mars Temperature DataLinks to an external site. site. Note that the URL is https://data-class-mars-challenge.s3.amazonaws.com/Mars/index.html.

Scrape the data in the HTML table. To do so, choose one of two ways. The first, simpler way is to use Pandas's read_html method. The second, slightly more challenging way is to manually scrape the data by using Splinter and Beautiful Soup. We highly encourage you to choose the latter to reinforce your scraping skills.

Assemble the scraped data into a Pandas DataFrame. The columns should have the same headings as the table on the website. Here’s an explanation of the column headings:

The id heading: The identification number of a single transmission from the Curiosity rover. The terrestrial_date heading: The date on Earth. The sol heading: The number of elapsed sols (Martian days) since Curiosity landed on Mars. The ls heading: The solar longitude. The month heading: The Martian month. The min_temp heading: The minimum temperature, in Celsius, of a single Martian day (sol). The pressure heading: The atmospheric pressure at Curiosity's location. Examine the data types of all the DataFrame columns. If necessary, cast (or convert) the data to the appropriate datetime, int, or float data types.

How many months exist on Mars?

How many Martian (and not Earth) days' worth of data exist in the scraped dataset?

What are the coldest and the warmest months on Mars (at the location of Curiosity)? Get the answer by averaging the minimum daily temperature of all the months. Plot the results as a bar chart.

Which months have the lowest and the highest atmospheric pressure on Mars? Get the answer by averaging the daily atmospheric pressure of all the months. Plot the results as a bar chart.

About how many terrestrial (Earth) days exist in a Martian year? That is, in the time that Mars circles the Sun once, how many days elapse on Earth? Visually estimate the result by plotting the daily minimum temperature.

Export the DataFrame to a CSV file.