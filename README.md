# web-scraping-challenge

# Requirements
This challenge consists of two technical products; and, the following deliverables have to be submitted:
1. Deliverable 1: Scrape titles and preview text from Mars news articles.
2. Deliverable 2: Scrape and analyze Mars weather data, which exists in a table.

# Part 1: Scrape Titles and Preview Text from Mars News
In the Jupyter Notebook, the following steps are to be followed to scrape the Mars News website.

1. Use automated browsing to visit the `Mars news site` (https://static.bc-edx.com/data/web/mars_news/index.html). Inspect the page to identify which elements to scrape.
2. Create a Beautiful Soup object and use it to extract text elements from the website.
3. Extract the titles and preview text of the news articles that you scraped. Store the scraping results in Python data structures as follows:
  a. Store each title-and-preview pair in a Python dictionary and, give each dictionary two keys: title and preview. 
  b. Store all the dictionaries in a Python list.
  c. Print the list in the notebook.

![2](https://github.com/Pooja14n/web-scraping-challenge/assets/144713762/4501c686-fd24-420c-a97b-7eb8b5d667bc)

# Part 2: Scrape and Analyze Mars Weather Data
In the Jupyter Notebook the following steps are to be followed to scrape and analyze Mars weather data.

1. Use automated browsing to visit the `Mars Temperature Data Site`. Inspect the page to identify which elements to scrape. Note that the URL is `https://static.bc-edx.com/data/web/mars_facts/temperature.html`.
2. Create a Beautiful Soup object and use it to scrape the data in the HTML table, using Beautiful Soup.

![3](https://github.com/Pooja14n/web-scraping-challenge/assets/144713762/b5d05102-5ebd-46ac-b2c6-a83f07f2b48a)

3. Assemble the scraped data into a Pandas DataFrame. The columns should have the same headings as the table on the website. Here’s an explanation of the column headings:
`id`: the identification number of a single transmission from the Curiosity rover
`terrestrial_date`: the date on Earth
`sol`: the number of elapsed sols (Martian days) since Curiosity landed on Mars
ls: the solar longitude
`month`: the Martian month
`min_temp`: the minimum temperature, in Celsius, of a single Martian day (sol)
`pressure`: The atmospheric pressure at Curiosity's location

![4](https://github.com/Pooja14n/web-scraping-challenge/assets/144713762/f7565791-7822-43c6-9bbb-d5ddd45863dc)

4. Examine the data types that are currently associated with each column. If necessary, cast (or convert) the data to the appropriate datetime, int, or float data types.

![5](https://github.com/Pooja14n/web-scraping-challenge/assets/144713762/18fc6703-634d-46a4-b74e-c7aeb50e9646)

![6](https://github.com/Pooja14n/web-scraping-challenge/assets/144713762/06fd80dc-5ff6-45bf-9f63-c6ff903f6c6a)

5. Analyze the dataset by using Pandas functions to answer the following questions:
  a. How many months exist on Mars?
![7](https://github.com/Pooja14n/web-scraping-challenge/assets/144713762/350d5237-dd53-412a-8663-c3b670b6ebd6)

  b. How many Martian (and not Earth) days worth of data exist in the scraped dataset?
![8](https://github.com/Pooja14n/web-scraping-challenge/assets/144713762/1692c2d4-5590-414a-b023-777ec6ec929d)

  c. What are the coldest and the warmest months on Mars (at the location of Curiosity)? To answer this question:
     i. Find the average minimum daily temperature for all of the months.
   ![9](https://github.com/Pooja14n/web-scraping-challenge/assets/144713762/3ba17ba2-18dd-4bc4-8a5a-7aab29a78190)
   
     ii. Plot the results as a bar chart.
   ![10](https://github.com/Pooja14n/web-scraping-challenge/assets/144713762/0112c745-8276-4adf-b9b7-c96fc87ecea5)

   ![11](https://github.com/Pooja14n/web-scraping-challenge/assets/144713762/792fc57f-2750-4489-a17e-801b97dc1077)

  d. Which months have the lowest and the highest atmospheric pressure on Mars? To answer this question:
     i. Find the average daily atmospheric pressure of all the months.
   ![12](https://github.com/Pooja14n/web-scraping-challenge/assets/144713762/97716bc7-0c93-45e4-a56c-8a0a87dc68c4)
   
     ii. Plot the results as a bar chart.
   ![13](https://github.com/Pooja14n/web-scraping-challenge/assets/144713762/0a75bd13-3a2e-43f5-9699-d283b8fe7296)
   
  e. About how many terrestrial (Earth) days exist in a Martian year? To answer this question:
     i. Consider how many days elapse on Earth in the time that Mars circles the Sun once.
     ii. Visually estimate the result by plotting the daily minimum temperature.
     ![14](https://github.com/Pooja14n/web-scraping-challenge/assets/144713762/bd0fa653-98eb-46dd-8c46-b44057a9c330)
     
6. Export the DataFrame to a CSV file.
