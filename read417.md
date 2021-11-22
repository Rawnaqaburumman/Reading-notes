# web scraping:
- process of using bots to extract content and data from a website.

- Unlike screen scraping, which only copies pixels displayed onscreen, web scraping extracts underlying HTML code and, with it, data stored in a database. The scraper can then replicate entire website content elsewhere.

- Web scraping is used in a variety of digital businesses that rely on data harvesting. Legitimate use cases include:

    - Search engine bots crawling a site, analyzing its content and then ranking it.
    - Price comparison sites deploying bots to auto-fetch prices and product descriptions for allied seller websites.
   - Market research companies using scrapers to pull data from forums and social media (e.g., for sentiment analysis).

- Web scraping is also used for illegal purposes, including the undercutting of prices and the theft of copyrighted content. An online entity targeted by a scraper can suffer severe financial losses, especially if it’s a business strongly relying on competitive pricing models or deals in content distribution.

- Scraper tools and bots Web scraping tools are software (i.e., bots) programmed to sift through databases and extract information. A variety of bot types are used, many being fully customizable to:

    - Recognize unique HTML site structures
    - Extract and transform content
    - Store scraped data
    - Extract data from APIs
    
    ## Python Code

We start by importing the following libraries.

```
import requests
import urllib.request
import time
from bs4 import BeautifulSoup
```
Next, we set the url to the website and access the site with our requests library.

```
url = 'http://web.mta.info/developers/turnstile.html'
response = requests.get(url)
```

If the access was successful, you should see the following output:

![4](https://miro.medium.com/max/414/1*fyqRGzG8IbhhjxF2Q5MU_Q.png)

Next we parse the html with BeautifulSoup so that we can work with a nicer, nested BeautifulSoup data structure. If you are interested in learning more about this library, check out the BeatifulSoup documentation.

```
soup = BeautifulSoup(response.text, “html.parser”)
```

We use the method .findAll to locate all of our <a> tags.

```
soup.findAll('a')
```

This code gives us every line of code that has an < a > tag. The information that we are interested in starts on line 38 as seen below. That is, the very first text file is located in line 38, so we want to grab the rest of the text files located below.

![5](https://miro.medium.com/max/582/1*G6YulYb5rczkVvmn7nbQ6g.png)

Next, let’s extract the actual link that we want. Let’s test out the first link.

```
one_a_tag = soup.findAll(‘a’)[38]
link = one_a_tag[‘href’]
```
This code saves the first text file, ‘data/nyct/turnstile/turnstile_180922.txt’ to our variable link. The full url to download the data is actually ‘http://web.mta.info/developers/data/nyct/turnstile/turnstile_180922.txt’ which I discovered by clicking on the first data file on the website as a test. We can use our urllib.request library to download this file path to our computer. We provide request.urlretrieve with two parameters: file url and the filename. For my files, I named them “turnstile_180922.txt”, “turnstile_180901”, etc.

```
download_url = 'http://web.mta.info/developers/'+ link
urllib.request.urlretrieve(download_url,'./'+link[link.find('/turnstile_')+1:])
```

Last but not least, we should include this line of code so that we can pause our code for a second so that we are not spamming the website with requests. This helps us avoid getting flagged as a spammer.

```
time.sleep(1)
```

Now that we understand how to download a file, let’s try downloading the entire set of data files with a for loop. The code below contains the entire set of code for web scraping the NY MTA turnstile data.

```
# Import libraries
import requests
import urllib.request
import time
from bs4 import BeautifulSoup

# Set the URL you want to webscrape from
url = 'http://web.mta.info/developers/turnstile.html'

# Connect to the URL
response = requests.get(url)

# Parse HTML and save to BeautifulSoup object¶
soup = BeautifulSoup(response.text, "html.parser")

# To download the whole data set, let's do a for loop through all a tags
line_count = 1 #variable to track what line you are on
for one_a_tag in soup.findAll('a'):  #'a' tags are for links
    if line_count >= 36: #code for text files starts at line 36
        link = one_a_tag['href']
        download_url = 'http://web.mta.info/developers/'+ link
        urllib.request.urlretrieve(download_url,'./'+link[link.find('/turnstile_')+1:]) 
        time.sleep(1) #pause the code for a sec
    #add 1 for next line
    line_count +=1
```
