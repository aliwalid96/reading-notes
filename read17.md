# Web scraping
Web scraping is a technique to automatically access and extract large amounts of information from a website, which can save a huge amount of time and effort.

In this article, we will go through an easy example of how to automate downloading hundreds of files from the New York MTA. This is a great exercise for web scraping beginners who are looking to understand how to web scrape.

after download the data there  hundreds of .txt files exist on the site. Below is a snippet of what some of the data looks like.
## inspecting the website
The first thing that we need to do is to figure out where we can locate the links to the files we want to download inside the multiple levels of HTML tags. Simply put, there is a lot of code on a website page and we want to find the relevant pieces of code that contains our data
and there will be a html page 

## Python Code

~~~
import requests
import urllib.request
import time
from bs4 import BeautifulSoup

url = 'http://web.mta.info/developers/turnstile.html'
response = requests.get(url)

soup = BeautifulSoup(response.text, “html.parser”)

~~~

We use the method .findAll to locate all of our <a> tags.
~~~
soup.findAll('a')


one_a_tag = soup.findAll(‘a’)[38]
link = one_a_tag[‘href’]

time.sleep(1)

~~~

This code saves the first text file, ‘data/nyct/turnstile/turnstile_180922.txt’ to our variable link. 

