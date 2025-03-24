# Web Scraping Workshop

This repository contains files associated with a workshop on web scraping created for the University of Oklahoma's Digital Humanities Community of Practice.

There are many ways to scrape information from the internet. You can just copy information from your browser window and paste it into your favorite word processing or spreadsheet program. A **spider** can crawl sites or collections of sites and retrieve specific information according to the instructions you give it. [Scrapy](https://docs.scrapy.org/en/latest/intro/tutorial.html) is a Python module for building spiders. You can also retrieve information using command line tools like [`wget`](https://www.gnu.org/software/wget/). Proprietary no-code or low-code services are also available (see below).

This workshop is about using the [BeautifulSoup](https://www.crummy.com/software/BeautifulSoup/) module for Python to extract and format specific information from a set of web pages.

The Jupyter Notebook for this workshop is available on Google Colab at <https://colab.research.google.com/drive/1IjHOhmEKamnqMP8VCOY3uUzcjkTkHikW#scrollTo=p3byaK2jEObF>. If you want to run the code cells, please do so in a copy of the file.

## Scenario

In this tutorial, we'll imagine that our task is to assemble a table of basic information about the universities in the [Southeastern Conference (SEC)](https://www.secsports.com/). We *could* go to the websites of all sixteen organizations and hunt down everything we need to know, but that would take hours or even days. We need the information **now**.

We'll build a scraper that will do the following:

1. Request the main SEC page at <https://en.wikipedia.org/wiki/Southeastern_Conference>
2. Find the table on all 16 member institutions on that page
3. Build a list of names of institutions and links to their individual pages
4. Request each of the individual pages
5. Find the "infobox" table on each individual page
6. Parse the information in the "infobox" table
7. Scrape the "infobox" information into Pandas dataframes
8. Consolidate the "infobox" information for all 16 institutions
9. Save the information in an Excel workbook and a CSV file.

By the end of this tutorial, we'll have covered the most common techniques in web scraping, but there is much, much more to learn. If you're at OU, the best place to start is University Libraries' [Digital Scholarship and Data Services](https://libraries.ou.edu/units/digital-scholarship-and-data-services#:~:text=Digital%20Scholarship%20%40%20OU%20Libraries%20supports%20collaborative%2C%20cross-disciplinary,that%20build%20on%20traditional%20research%20and%20teaching%20methods.). They offer one-on-one consultations and on-request workshops.

## Other Resources on Web Scraping

### Free and Open Source

- [Beautiful Soup Documentation](https://www.crummy.com/software/BeautifulSoup/bs4/doc/)
- [Python for Digital Humanities Tutorial on BeautifulSoup](https://www.youtube.com/watch?v=_tdW6n7lUX4)
- [Tutorials from the Programming Historian](https://programminghistorian.org/en/lessons/?topic=web-scraping)
- [Scrapy Tutorial](https://docs.scrapy.org/en/latest/intro/tutorial.html)

### Proprietary Applications

- [Browse.ai](https://www.browse.ai/)
- [Octoparse](https://www.octoparse.com/)
- [Scrapfly](https://scrapfly.io/)
