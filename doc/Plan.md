# Web Scraper Development Plan

## Requirment Analysis

* Basic flow of the program
  * When running the program, the user must provide a starting url
  * That url will be put in some data structure so the program knows not to visit that page again
    * Data structure will likely be a hash map
  * The program will take that url, and fetch the HTML page
  * The program will read the HTML page and parse the data
  * When the program finds another url, it will attempt to fetch the HTML page coorelated to that url
    * If the attempt fails, the program will print an error and continue
  * If the program successfully fetches the HTML page, the program will print the url
    * Url's will be printed with indents based on what level of depth they're on
    * First url has no indents, all urls on that page have one indent, so on
  * The program will stop after it has visited all urls within range.

* What I know how to do in Java
  * Parse string
  * Print to the console
  * Employ multithreading
  * Create and write in files

* What I know I don't know
  * How to fetch HTML data with a URL
  * How to extract specific data from a variety of pages

* What i don't know I don't know:
  *

* Data used by the program
  * url - string - provided by the user
  * visited urls - hash table - created and managed by the program

* Algorithms needed
  * An algorithm to fetch the html page using a url
  * An algorithm to read the html page and scrape the desired data
  * An algorithm that formats the data and prints it to the console

## Design

### Basic Overview

The program will include one class. That class will have two functions (not including main). One method will be used to make requests to the web using the supplied
url. The other will be used to parse data out of the html page. The `main` method will contain a loop that continually runs as long as there are urls to make fetch
requests with.

