# movie_recomendation_based_on_emotion

This project provides a Python script that recommends movies based on a user-inputted emotion. It leverages web scraping to fetch movie titles from IMDb, mapping specific emotions to movie genres to deliver relevant recommendations.

## Introduction

Movies have a powerful ability to evoke and explore a wide range of emotions, resonating deeply with audiences. This Python script aims to provide movie recommendations tailored to a user's current emotional state. By correlating emotions with specific movie genres, it scrapes IMDb for top movie titles within those genres.

## How it Works

The script operates by:
1.  **Mapping Emotions to Genres**: A predefined dictionary links common emotions (e.g., "Drama", "Action") to specific IMDb genre search URLs.
2.  **Web Scraping IMDb**: When an emotion is entered, the script constructs a URL to IMDb's movie search page for the corresponding genre.
3.  **Fetching and Parsing**: It then sends an HTTP request to IMDb, retrieves the HTML content, and uses Beautiful Soup and LXML to parse the HTML.
4.  **Extracting Movie Titles**: The parsed HTML is searched for movie titles, which are then extracted and presented to the user.

## Features

* **Emotion-based Recommendations**: Get movie suggestions based on a specified emotion.
* **IMDb Integration**: Scrapes real-time movie data from IMDb.
* **Simple Command-Line Interface**: Easy to use by running the script and providing an emotion as input.


# Libraries Used
requests: An elegant and simple HTTP library for Python, used to make requests to web servers (e.g., IMDb) to retrieve their HTML content.

BeautifulSoup (from bs4): A Python library designed for pulling data out of HTML and XML files. It works with a parser to provide idiomatic ways of navigating, searching, and modifying the parse tree.

lxml: A highly feature-rich and easy-to-use library for processing XML and HTML data. It is often used as a fast and powerful parser in conjunction with BeautifulSoup.

re: Python's built-in module for regular expressions, used here for pattern matching to find specific elements (like movie title links) within the HTML.

## Installation

To run this script, you need to have Python installed. Additionally, you'll need the `requests`, `beautifulsoup4`, and `lxml` libraries.

Open your terminal or command prompt and run the following commands to install the required libraries:

```bash
pip install beautifulsoup4
pip install lxml
pip install requests
