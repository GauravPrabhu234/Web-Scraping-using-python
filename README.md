# Web-Scraping-using-python

# What is Web Scraping 
Web scraping is a technique used to extract data from websites by sending requests to the server, retrieving the web pages, and parsing the HTML content to extract the necessary information.

# Overview of the project
In this project, I will walk through the process of web scraping from Amazon’s Best Sellers page in the Teaching & Education category to collect data about the top 50 authors and their ratings.

# Necessary Libraries
requests: to send HTTP requests and retrieve the web pages.
BeautifulSoup: to parse and extract information from the HTML content.
pandas: to organize and save the extracted data in a tabular format.


If you don't have beautifulSoup library then install it in command prompt using the command:- pip install beautifulsoup4

If you don't have requests library then install it in command prompt using the command :- pip install requests

If you don't have pandas  library then install it in command prompt using the command :- pip install pandas

# Steps for performing this project 
# Step 1: Understanding the Target URL and Pagination
We are targeting the Amazon Best Sellers page in the Teaching & Education category. Amazon’s pagination allows us to navigate through multiple pages of results.
The URL :- https://www.amazon.in/gp/bestsellers/books/4149461031/ref=zg_bs_pg_1?ie=UTF8&pg=1

# Step 2: Set Up the HTTP Request
To scrape the content from Amazon, we first need to send a request to the server and retrieve the HTML content of the page. We also need to mimic a real browser to avoid being blocked by Amazon, which is why we always need to include a User-Agent header in the request. 

# Step 3: Iterate Over Pages to Collect Data
We will loop through the first three pages to collect data for the top 50 books (assuming each page displays around 20 items). On each page, we will extract the author’s name and rating.

# Step 4: Store and Save the Data
After collecting the data, we will store it in a Pandas DataFrame and save it to a CSV file.

