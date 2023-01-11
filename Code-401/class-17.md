## Web Scraping

### Web Scrape with Python in 4 Minutes

- Web scraping is a technique to automatically access and extract large amounts of information from a website, which can save a huge amount of time and effort.
- Important notes about web scraping:
  - Read through the website's Terms and Conditions to understand how you can legally use the data. Most sites prohibit you from using the data for commercial purposes.
  - Make sure you are not downloading data at too rapid a rate because this may break the website. You may potentially be blocked from the site as well.
- The first step is to figure out where to find the links to the files we want to download, within multiple levels of HTML tags

### How to Scrape Website Without Getting Blocked

- Web scraping needs to be performed responsibly so that it does not have a detrimental effect on the sites being scraped.
- Best practices:
  - respect robots.txt
    - it specifies rules for good behavior, such as how frequently you can scrape, which pages allow scraping and which don't
  - crawl slowly, don't slam the website all at once
  - don't follow the same crawling pattern
  - make requests through proxies and rotate them as needed
  - Rotate User Agents and corresponding HTTP Request Headers between requests
  - Use a headless browser like Puppeteer, Selenium or Playwright
  - Beware of Honey Pot Traps
  - Check if Website is Changing Layouts
  - Avoid scraping data behind a login
  - Use Captcha Solving Services
  - How can websites detect and block web scraping?

### Sources

[Web Scrape with Python in 4 Minutes](https://towardsdatascience.com/how-to-web-scrape-with-python-in-4-minutes-bc49186a8460)<br>
[What is Web Scraping?](https://en.wikipedia.org/wiki/Web_scraping)<br>
[How to Scrape Website Without Getting Blocked](https://www.scrapehero.com/how-to-prevent-getting-blacklisted-while-scraping/)<br>
[Track Amazon Prices](https://www.youtube.com/watch?v=Bg9r_yLk7VY)<br>
[Beautiful Soup](https://www.crummy.com/software/BeautifulSoup/)<br>