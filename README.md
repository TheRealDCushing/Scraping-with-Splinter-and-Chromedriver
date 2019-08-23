# Scraping with Splinter and Chromedriver


We are tasked with creating a program that scrapes NASA's website, and others, to retrieve pictures.
Doing this requires the use of Splinter, BeautifulSoup, and pandas. 

Splinter is a library that works in conjunction with a program called "chromedriver" to operate a
remote instance of google chrome via commands that can be run from the console or a Jupyter Notebook.
(To run splinter, we must have chromedriver installed on our computer, and be able to reference the
folder in which it is contained. In the bootcamp, we were instructed to copy the chromedriver file 
into each of the folders of the assignments or exercises we worked on, but I placed it in a global
folder much higher up so I can easily reference it at any time).

We set the URLs to the websites of interet that we want to livescrape. Then, we use BeautifulSoup
to isolate the "src=..." and so extract the source of the image we want to use for our purposes.

Pandas makes it especially easy to scrape tables on websites we find interesting, so it was used
instead of beautifulsoup wherever possible. 

A loop was utilized in conjunction with chromedriver to retrieve all of the images, in this case
by cleverly referencing the <h3> tag, since that was used exclusively in conjunction with the categories
of interest.
