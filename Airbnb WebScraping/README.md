# Airbnb Web Scraping
#### Main Objective
Conduct an exhaustive scraping on all stays available at Airbnb in the major cities of France, and perform a supply-demand analysis to come up with a supply management scheme to accurately meet market's need. Accordingly, this project will be divided into multiple tasks.

#### Task 1 - Problem Definition
A friend of mine is coming to Paris, France to undego the Data Analytics bootcamp at Ironhack. He required a debrief of all avaiable stays at Airbnb based on a pre-defined set of search filters. To kickstart our web scraping, we need to answer the following questions:
- How is the website structured?
- What data is available for the user to scrape?
- How are the URL's structured?
- What is the best approach to scrape the website?

#### Tools Used
- Python
  - Libraries:
    - requests
    - json
    - bs4
    - pandas
    - numpy
    - re
    - time

#### Process
- Airbnb: API based web-server
- 1 API contained the main key that was holding all the research output
- For a user-interactive search, 10 user inputs (Filters) are required
- As soon as I got the request URL, a <Response 400> message appears
- I had to included HTTP request headers to avoid suspicions to the web server of bot-like behavior (non-organic request approach) and avoid having them block the web scraping process
- I had to remove the Federated Search ID and Source keys from URL as they were changing after each scraping session 
- I had to remove cookies to be able to display a unique concatenated DF
- The output was matching the web server search via an Incognito Mode

#### Results
