# Web Scraping Workshop

This repository contains files associated with a workshop on web scraping created by [Sam Huskey](https://sjhuskey.info/) for the University of Oklahoma's Digital Humanities Community of Practice.

This workshop is about using the [BeautifulSoup](https://www.crummy.com/software/BeautifulSoup/) module for Python to extract and format specific information from a set of web pages. It demonstrates some key functions and techniques, but there are many more advanced operations that cannot be covered in this brief forum.

A version of the Jupyter Notebook for this workshop is available on [Google Colab](https://colab.research.google.com/drive/1IjHOhmEKamnqMP8VCOY3uUzcjkTkHikW#scrollTo=p3byaK2jEObF) at <https://bit.ly/4j2bIWO>. If you want to run the code cells, please do so in a copy of the file.

By the end of this tutorial, we'll have covered the most common techniques in web scraping, but there is much, much more to learn. If you're at OU, the best place to start is University Libraries' [Digital Scholarship and Data Services](https://libraries.ou.edu/units/digital-scholarship-and-data-services#:~:text=Digital%20Scholarship%20%40%20OU%20Libraries%20supports%20collaborative%2C%20cross-disciplinary,that%20build%20on%20traditional%20research%20and%20teaching%20methods.). They offer one-on-one consultations and on-request workshops.

## Other Resources on Web Scraping

There are many ways to scrape information from the internet. 

You can just copy information from your browser window and paste it into your favorite word processing or spreadsheet program. That's the best approach if you just need to get a small amount of information from one or two pages. Beyond that, you should consider automating your scraping with one or more of the following tools.

### BeautifulSoup

This workshop focuses on using the popular `BeautifulSoup` module for Python. It comes with many predefined functions for handling common tasks in webscraping. It's particularly good at navigating the structure of web pages.

- [Beautiful Soup Documentation](https://www.crummy.com/software/BeautifulSoup/bs4/doc/): The documentation includes a walkthrough of the different methods for connecting to web sites and extracting information from them.
- [Python for Digital Humanities Tutorial on BeautifulSoup](https://www.youtube.com/watch?v=_tdW6n7lUX4): This is just one of the many tutorials available on WJB Mattingly's YouTube channel for digital humanities computing.

### Scrapy

A **spider** can crawl sites or collections of sites and retrieve specific information according to the instructions you give it. [Scrapy](https://scrapy.org/) is a Python module for building spiders. 

- [Official Scrapy Tutorial](https://docs.scrapy.org/en/latest/intro/tutorial.html)
- [Digital Ocean Scrapy Tutorial](https://www.digitalocean.com/community/tutorials/how-to-crawl-a-web-page-with-scrapy-and-python-3)
- [Scrapfly Tutorial on Scrapy](https://scrapfly.io/blog/web-scraping-with-scrapy/)

### Command Line Tools

You can also retrieve information using command line tools like [`wget`](https://www.gnu.org/software/wget/). The [Programming Historian](https://programminghistorian.org/) site has some tutorials to help:

- [Automated Downloading with Wget](https://programminghistorian.org/en/lessons/automated-downloading-with-wget)
- [Applied Archival Downloading with Wget](https://programminghistorian.org/en/lessons/applied-archival-downloading-with-wget)

### Proprietary Applications

Many commercial services offer low-code or no-code solutions for scraping content from the interent:

- [Browse.ai](https://www.browse.ai/)
- [Octoparse](https://www.octoparse.com/)
- [Scrapfly](https://scrapfly.io/)

_____
## Setting Up the Environment

### Using Conda
To recreate the Python environment used in this tutorial, run this in the Terminal:
```bash
conda env create -f [environment.yml](http://_vscodecontentref_/8)
```

### Using Pip

To use Pip to recreate the Python environment used in this tutorial, run this in the Terminal
```bash
python -m venv venv
source venv/bin/activate  
# On Windows: venv\Scripts\activate
pip install -r [requirements.txt](http://_vscodecontentref_/9)
```
