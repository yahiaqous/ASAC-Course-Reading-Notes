# Web Scraping

Web scraping is a technique to automatically access and extracts large amounts of information from a website, which can save a huge amount of time and effort.

Turnstile data is compiled every week from May 2010 to the present, so hundreds of .txt files exist on the site (<http://web.mta.info/developers/turnstile.html>).

&nbsp;

## Techniques

- Human copy-and-paste

- Text pattern matching

- HTTP programming

- HTML parsing

- DOM parsing

- Vertical aggregation

- Semantic annotation recognizing

- Computer vision web-page analysis

&nbsp;

## Web Scraping best practices to follow to scrape without getting blocked

- Respect Robots.txt

- Make the crawling slower, do not slam the server, treat websites nicely

- Do not follow the same crawling pattern

- Make requests through Proxies and rotate them as needed

- Rotate User Agents and corresponding HTTP Request Headers between requests

- Use a headless browser like Puppeteer, Selenium, or Playwright

- Beware of Honey Pot Traps

- Check if Website is Changing Layouts

- Avoid scraping data behind a login

- Use Captcha Solving Services

- How can websites detect web scraping?

- How do you find out if a website has blocked or banned you?

&nbsp;

## Inspecting the Website

The first thing that we need to do is to figure out where we can locate the links to the files we want to download inside the multiple levels of HTML tags. Simply put, there is a lot of code on a website page and we want to find the relevant pieces of code that contain our data.

### **Python Code**

- We start by importing the following libraries.

        import requests
        import urllib.request
        import time
        from bs4 import BeautifulSoup

- Next, we set the URL to the website and access the site with our requests library.

        url = 'http://web.mta.info/developers/turnstile.html'
        response = requests.get(url)

- Next we parse the HTML with BeautifulSoup so that we can work with a nicer, nested BeautifulSoup data structure.

        soup = BeautifulSoup(response.text, “html.parser”)

- We use the method .findAll to locate all of our < a > tags

        soup.findAll('a')
