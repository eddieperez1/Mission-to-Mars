# Mission-to-Mars

## Overview of Project

### Installation 

The following modules were used to create and run the code in this project. Install mongodb and mongo compass onto your computer and the following modules into your python environment.

```
pip install splinter
```
```
pip install webdriver_manager
```
```
pip install bs4
```
```
pip install pymongo
```
```
pip install flask
```
```
pip install flask_pymongo
```
```
pip install pandas
```
```
pip install datatime
```
### Outline

This project's design is to help a client by web scraping data from several websites and show it on a web page. The data will be information, news and images of Mars. Splinter will be used to web scrape the websites then the data will be stored in a mongo database. Next the data will be displayed on a web page using flask.

## Results

### Deliverable 1: Scrape Full-Resolution Mars Hemisphere Images and Titles 

In the module, the mars news from [redplanetscience.com](https://redplanetscience.com/), featured image from [spaceimages-mars.com](https://spaceimages-mars.com), and mars facts from [galaxyfacts-mars.com](https://galaxyfacts-mars.com) were scraped. In this project, the mars hemisphere images and titles from [marshemispheres.com](https://marshemispheres.com) were scraped. 

### Deliverable 2:  Update the Web App with Mars’s Hemisphere Images and Titles

In the module, scraping.py was created to store the code for scraping the websites from deliverable 1. scraping.py has a function for each web scrape and combines it into one function scrape_all. This scrape_all function was added to the app.py to run the website using flask. This project has index.html with a div that holds the images, and text scraped from the web scrape. Then the flask app was run and data was shown on the localhost web page.  

### Deliverable 3: Add Bootstrap 3 Components

This project stylized the web page using Bootstrap 3 and CSS classes. For example, the mars facts is a table with table-hover class and the mars hemispheres were put side by side using 
```
class = 'col-md-3'
```

## Summary

### Conclusion

The project successfully displays the mars information, news and images that the client wanted on a web page.

### Usage

To use this code, run app.py and open localhost:5000 on a browser.

#### The web page before scraping

![Mission to Mars Before Scraping](/screenshots/mission_to_mars_before.PNG)

#### The web page after scraping

![Mission to Mars After Scraping](/screenshots/mission_to_mars_after.PNG)
