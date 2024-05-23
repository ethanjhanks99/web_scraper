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
